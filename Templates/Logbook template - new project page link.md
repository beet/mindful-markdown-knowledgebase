<%*
  var noteTitle = await tp.system.prompt("Please enter the project name");
  var noteTitle = 'Project - ' + noteTitle;
-%>
[[Project notes/<% noteTitle %>|<% noteTitle %>]]