<%*
  var issueNumber = await tp.system.prompt("Please enter the issue number, like AB-1234")
  var issueName = await tp.system.prompt("Please enter the issue name")
  var noteTitle = "Issue " + issueNumber + " - " + issueName;
-%>
[[Issue notes/<% noteTitle %>|<% noteTitle %>]]