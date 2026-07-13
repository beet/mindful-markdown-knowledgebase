<%*
  var title = await tp.system.prompt("Please enter the meeting title")
  var date = tp.date.now('YYYY-MM-DD')
  var meetingTitle = "Meeting " + date + " - " + title;
-%>
[[Meeting notes/<% meetingTitle %>|<% meetingTitle %>]]