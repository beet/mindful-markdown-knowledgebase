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

## Weekly reviews

<%* var week = monthStart; -%>
- [[Weekly review <% week.format('YYYY-[W]WW') %>]]
- [[Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [[Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [[Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [[Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]
- [[Weekly review <% week.add(1, 'week').format('YYYY-[W]WW') %>]]

> [!Info] Drop target
> Collect bullet points from the weekly reviews here, then move down into the sections below.


---

### Projects


### Meetings


### Other


## Goals

Set your goals for this coming month in [[Monthly notes/<% thisMonth.format('YYYY-MM') %>|<% thisMonth.format('MMMM YYYY') %>]].
