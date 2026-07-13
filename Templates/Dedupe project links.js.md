<%*
// ```javascript
const editor = app.workspace.activeLeaf.view.editor;
const selection = editor.getSelection();

const groups = new Map();
const linkRe = /\[\[[^\]]+\]\]/;

for (const raw of selection.split('\n')) {
  const stripped = raw.replace(/^\s*[-*+]\s*/, '');
  const m = stripped.match(linkRe);
  if (!m) continue;
  const link = m[0];
  const prefix = stripped.slice(0, m.index).trim();
  if (!groups.has(link)) groups.set(link, []);
  groups.get(link).push(prefix);
}

const out = [];
for (const [link, prefixes] of groups) {
  out.push(`- ${link}`);
  const seen = new Set();
  for (const p of prefixes) {
    if (!p || seen.has(p)) continue;
    seen.add(p);
    out.push(`    - ${p}`);
  }
}

tR += out.join('\n');
//```
%>