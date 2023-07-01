<%* var date = moment(tp.file.title); -%>
# <% date.format('dddd YYYY-MM-DD') %>

```tasks
due <% date.format('YYYY-MM-DD') %>
not done
path does not include Daily notes/<% date.format('YYYY-MM-DD') %>
```

```tasks
done <% date.format('YYYY-MM-DD') %>
path does not include Daily notes/<% date.format('YYYY-MM-DD') %>
```

## ⏰ Weekly goals

```tasks
path includes Weekly notes/<% date.format('YYYY-[W]WW') %>
```

## 🎯 Monthly goals

```tasks
path includes Monthly notes/<% date.format('YYYY-MM') %>
```

---

