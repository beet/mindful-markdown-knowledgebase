<%*
  // The title is the _current_ month, like "Monthly review 2023-11"
  var prevMonth = moment(tp.file.title).subtract(1, 'M');
  var thisMonth = moment(tp.file.title);
  var nextMonth = moment(tp.file.title).add(1, 'M');
  var monthStart = moment(thisMonth).startOf('month');
-%>
# Monthly review for <% thisMonth.format('MMMM YYYY') %>

[[Monthly reviews/Monthly review <% prevMonth.format('YYYY-MM') %>|⬅️ Previous]] | [[Monthly reviews/Monthly review <% nextMonth.format('YYYY-MM') %>|Next  ➡️]]

Created <% moment().format('YYYY-MM-DD') %>

## 🏆 📌 Wins

## 🧠 📌 Learnings

## Weekly reviews

<%* var week = monthStart; -%>
- [ ] [[Weekly reviews/Weekly review <% week.format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [ ] [[Weekly reviews/Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]

> [!Info] Drop target
> Go through the weekly reviews above:
> * copy their bullet points and paste below
> * mark the check list as done
> * move them down into the sections below

📋 Paste here:

---

### 📌 Pressure


### 📌 Stress signals


### 📌 Projects


### 📌 Meetings


### 📌 Other


## 🥅 Goals

Set your goals for this coming month in [[Monthly notes/<% nextMonth.format('YYYY-MM') %>|<% nextMonth.format('MMMM YYYY') %>]].
