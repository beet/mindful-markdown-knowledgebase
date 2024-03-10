<%*
  var date = moment(tp.file.title);
  var weekStart = moment(tp.file.title).startOf('week');
  var weekEnd = moment(tp.file.title).endOf('week');
-%>
# Week <% date.format('W, MMMM YYYY') %>

[[Weekly notes/<% moment(tp.file.title).subtract(1, 'w').format('YYYY-[W]WW') %>|⬅️ Week <% moment(tp.file.title).subtract(1, 'w').format('WW') %>]] | [[Weekly notes/<% moment(tp.file.title).add(1, 'w').format('YYYY-[W]WW') %>|Week <% moment(tp.file.title).add(1, 'w').format('WW') %> ➡️]]

## 🥅 Weekly goals

- [ ] Task that will appear as a goal in the daily notes from week <% date.format('WW') %>

## 🔜 This week

```tasks
not done
(due after <% weekStart.subtract(1, 'day').format('YYYY-MM-DD') %>) OR (scheduled after <% weekStart.format('YYYY-MM-DD') %>)
(due before <% weekEnd.add(1, 'day').format('YYYY-MM-DD') %>) OR (scheduled before <% weekEnd.format('YYYY-MM-DD') %>)
sort by scheduled
sort by due
```

## 🎯 Monthly goals

[[Monthly notes/<% date.format('YYYY-MM') %>|<% date.format('MMMM YYYY') %> notes]]

```tasks
path includes Monthly notes/<% date.format('YYYY-MM') %>
sort by description
```
