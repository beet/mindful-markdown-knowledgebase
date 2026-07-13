---
status: WIP
started: <% tp.date.now('YYYY-MM-DD') %>
---
# <% tp.file.title %>

## Resources

* Links

## Do Today
```tasks
hide toolbar
not done
due today or scheduled today
path includes <% tp.file.title %>
```
## Overdue
```tasks
hide toolbar
not done
due before today or scheduled before today
path includes <% tp.file.title %>
```

## 📖 Logbook

* **<% tp.date.now('YYYY-MM-DD') %>:** started

### Meetings

```query
"<% tp.file.title %>"
path:"Meeting notes"
```

## ✅ Tasks

* [ ] Do something

## 🗒️ Notes

