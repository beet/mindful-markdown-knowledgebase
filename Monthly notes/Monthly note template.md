<%*
  var date = moment(tp.file.title);
  var monthStart = moment(tp.file.title).startOf('month');
  var monthEnd = moment(tp.file.title).endOf('month');
-%>
# <% date.format('MMMM YYYY') %>

[[Monthly notes/<% moment(tp.file.title).subtract(1, 'M').format('YYYY-MM') %>|⬅️ <% moment(tp.file.title).subtract(1, 'M').format('MMMM YYYY') %>]] | [[Monthly notes/<% moment(tp.file.title).add(1, 'M').format('YYYY-MM') %>|<% moment(tp.file.title).add(1, 'M').format('MMMM YYYY') %>  ➡️]]

- [[Yearly notes/<% date.format('YYYY') %>|<% date.format('YYYY') %>]]

## Monthly goals

- [ ] Task that will appear as a goal in the daily notes from <% date.format('MMMM YYYY') %>


## 🔜 This month

```tasks
not done
(due after <% monthStart.subtract(1, 'day').format('YYYY-MM-DD') %>) OR (scheduled after <% monthStart.format('YYYY-MM-DD') %>)
(due before <% monthEnd.add(1, 'day').format('YYYY-MM-DD') %>) OR (scheduled before <% monthEnd.format('YYYY-MM-DD') %>)
sort by scheduled
sort by due
```

<%* var week = monthStart; -%>
### Week <% week.format('WW') %>
```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
sort by description
```
### Week <% week.add(1, 'week').format('WW') %>

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
sort by description
```
### Week <% week.add(1, 'week').format('WW') %>

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
sort by description
```
### Week <% week.add(1, 'week').format('WW') %>

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
sort by description
```
### Week <% week.add(1, 'week').format('WW') %>

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
sort by description
```
### Week <% week.add(1, 'week').format('WW') %>

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
sort by description
```
