<%*
  // The title is the _current_ month, like "Monthly review 2023-11"
  // But reviewing the previous month.
  var monthBeforeLast = moment(tp.file.title).subtract(2, 'M');
  var prevMonth = moment(tp.file.title).subtract(1, 'M');
  var thisMonth = moment(tp.file.title);
  var nextMonth = moment(tp.file.title).add(1, 'M');
  var monthStart = moment(prevMonth).startOf('month');
  var monthEnd = moment(prevMonth).endOf('month');
-%>
# Monthly review for <% prevMonth.format('MMMM YYYY') %>

[[Monthly reviews/Monthly review <% prevMonth.format('YYYY-MM') %>|⬅️ Previous]] | [[Monthly reviews/Monthly review <% nextMonth.format('YYYY-MM') %>|Next  ➡️]]

Created <% moment().format('YYYY-MM-DD') %>

- **🏆 WINS:** 
- **🧠 LEARNINGS:** 

## Weekly reviews

<%* var week = monthStart; -%>
- [ ] [[Weekly reviews/Weekly review <% week.format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]

> [!Info] Drop target
> Go through the monthly reviews above:
> * copy their bullet points and paste below
> * mark the check list as done
> * move them down into the sections below

📋 Paste here:

---

### Projects


### Meetings


### Other


## 🥅 Goals

Set your goals for this coming month in [[Monthly notes/<% thisMonth.format('YYYY-MM') %>|<% thisMonth.format('MMMM YYYY') %>]].

<%* var week = prevMonth; -%>
### [[Weekly notes/<% week.format('YYYY-[W]WW') %>|Week <% week.format('WW') %>]]
```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
```
### [[Weekly notes/<% week.add(1, 'week').format('YYYY-[W]WW') %>|Week <% week.format('WW') %>]]

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
```
### [[Weekly notes/<% week.add(1, 'week').format('YYYY-[W]WW') %>|Week <% week.format('WW') %>]]

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
```
### [[Weekly notes/<% week.add(1, 'week').format('YYYY-[W]WW') %>|Week <% week.format('WW') %>]]

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
```
### [[Weekly notes/<% week.add(1, 'week').format('YYYY-[W]WW') %>|Week <% week.format('WW') %>]]

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
```
### [[Weekly notes/<% week.add(1, 'week').format('YYYY-[W]WW') %>|Week <% week.format('WW') %>]]

```tasks
path includes Weekly notes/<% week.format('YYYY-[W]WW') %>
```
