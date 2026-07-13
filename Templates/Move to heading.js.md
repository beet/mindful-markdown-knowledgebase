<%*
// ```javascript
const file = tp.config.active_file
const headings = this.app.metadataCache.getFileCache(file).headings;
const editor = app.workspace.activeLeaf.view.editor;
let content = "";
const isSelection = editor.somethingSelected();
const selection = editor.getSelection();
const line = editor.getLine(editor.getCursor().line);

// get the selection or line
if (isSelection) {
  content = selection;
} 
else {
  content = line
}

// Get the headers and prompt user to select
let headers = []

for (const heading of headings){
  headers.push(heading.heading);
}

let head = await tp.system.suggester(headers, headers);

var position; 
var existing;

// Get the existing content of the heading before adding the selected line 
for (var i = 0; i < headings.length; i++) { 
  var heading = headings[i]; 
  if (heading.heading == head) { 
    if (i == headings.length - 1) { 
      position = [heading.position.start.line, -1];
    } 
    else { 
      position = [heading.position.start.line, headings[i + 1].position.start.line]; 
    } 
  } 
} 

if (position) { 
  existing = tp.file.content.split("\n").slice(position[0], position[1]).join("\n");
  let matchHeader = existing.match(/#.*/gm)
  let matchBody = existing.replace(/#.*/gm,"").trimStart();
  
  // ask now if user wants to prepend or append to the section
  // let end = await tp.system.suggester(["prepend","append"],["prepend","append"]);
  
  // replace the original text with nothing and replace the existing content of the heading with the new prepended or appended text
  let oldText = tp.file.content.replace(content,"");

  // let newText

  /*
  if(end == "prepend"){
    newText = oldText.replace(existing,matchHeader[0] + "\n" + content + "\n" + matchBody);
  }

  if(end == "append"){
    newText = oldText.replace(existing,existing + "\n" + content);
  }
  */

  let newText = oldText.replace(existing,matchHeader[0] + "\n" + content + "\n" + matchBody);

  // replace the file with the new text
  await app.vault.modify(file,newText)
}
//```
%>
