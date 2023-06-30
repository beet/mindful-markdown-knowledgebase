<%* var date = moment(tp.file.title); -%>
# <% date.format('dddd YYYY-MM-DD') %>

[[Daily notes/<% moment(tp.file.title).subtract(1, 'd').format('YYYY-MM-DD') %>|⬅️ <% moment(tp.file.title).subtract(1, 'd').format('ddd YYYY-MM-DD') %>]] | [[Daily notes/<% moment(tp.file.title).add(1, 'd').format('YYYY-MM-DD') %>|<% moment(tp.file.title).add(1, 'd').format('ddd YYYY-MM-DD') %> ➡️]]

```tasks
hide toolbar
due <% date.format('YYYY-MM-DD') %>
not done
sort by description
sort by due
sort by scheduled
```
```tasks
hide toolbar
scheduled <% date.format('YYYY-MM-DD') %>
not done
sort by description
sort by due
sort by scheduled
```

```tasks
hide toolbar
done <% date.format('YYYY-MM-DD') %>
sort by description
sort by due
sort by scheduled
```

## 🔴 Overdue

```tasks
hide toolbar
not done
(due before <% date.format('YYYY-MM-DD') %>) OR (scheduled before <% date.format('YYYY-MM-DD') %>)
status.name regex does not match /progress|cancelled|forwarded|scheduling|question|important|star|quote|location|bookmark|info|savings|idea|pros|cons|fire|key|win|up|down/
sort by description
sort by due
sort by scheduled
```

## 🔜 Upcoming

```tasks
hide toolbar
not done
(due after <% date.format('YYYY-MM-DD') %>) OR (scheduled after <% date.format('YYYY-MM-DD') %>)
(due before <% date.isoWeekday("Saturday").format('YYYY-MM-DD') %>) OR (scheduled before this <% date.isoWeekday("Saturday").format('YYYY-MM-DD') %>)
sort by scheduled
sort by due
```

## 🥅 Weekly goals

[[Weekly notes/<% date.format('YYYY-[W]WW') %>|Week <% date.format('WW') %> notes]]

```tasks
hide toolbar
path includes Weekly notes/<% date.format('YYYY-[W]WW') %>
sort by description
```

## ✅ Tasks

- To **act well** in your given role, *this* is your **sphere of power**

## 📖 Logbook

- Started
