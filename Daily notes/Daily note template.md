<%* var date = moment(tp.file.title); -%>
# <% date.format('dddd YYYY-MM-DD') %>

[[Daily notes/<% moment(tp.file.title).subtract(1, 'd').format('YYYY-MM-DD') %>|⬅️ <% moment(tp.file.title).subtract(1, 'd').format('ddd YYYY-MM-DD') %>]] | [[Daily notes/<% moment(tp.file.title).add(1, 'd').format('YYYY-MM-DD') %>|<% moment(tp.file.title).add(1, 'd').format('ddd YYYY-MM-DD') %> ➡️]]

```tasks
due <% date.format('YYYY-MM-DD') %>
not done
path does not include Daily notes/<% date.format('YYYY-MM-DD') %>
```
```tasks
scheduled <% date.format('YYYY-MM-DD') %>
not done
path does not include Daily notes/<% date.format('YYYY-MM-DD') %>
```

```tasks
done <% date.format('YYYY-MM-DD') %>
path does not include Daily notes/<% date.format('YYYY-MM-DD') %>
```

## 🔴 Overdue

```tasks
not done
(due before <% date.format('YYYY-MM-DD') %>) OR (scheduled before <% date.format('YYYY-MM-DD') %>)
status.name regex does not match /progress|cancelled|forwarded|scheduling|question|important|star|quote|location|bookmark|info|savings|idea|pros|cons|fire|key|win|up|down/
```

### ⏰ Weekly goals

[[Weekly notes/<% date.format('YYYY-[W]WW') %>|Week <% date.format('WW') %> notes]]

```tasks
path includes Weekly notes/<% date.format('YYYY-[W]WW') %>
```

### 🎯 Monthly goals

[[Monthly notes/<% date.format('YYYY-MM') %>|<% date.format('MMMM YYYY') %> notes]]

```tasks
path includes Monthly notes/<% date.format('YYYY-MM') %>
```

## Log

