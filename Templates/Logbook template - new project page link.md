<%*
  var noteTitle = await tp.system.prompt("Please enter the project name");
  var noteTitle = 'PROJECT - ' + noteTitle;
-%>
[[Project notes/<% noteTitle %>|<% noteTitle %>]]