<%* var date = moment(tp.file.title); -%>
# <% date.format('MMMM YYYY') %>

[[Monthly notes/<% moment(tp.file.title).subtract(1, 'M').format('YYYY-MM') %>|⬅️ <% moment(tp.file.title).subtract(1, 'M').format('MMMM YYYY') %>]] | [[Monthly notes/<% moment(tp.file.title).add(1, 'M').format('YYYY-MM') %>|<% moment(tp.file.title).add(1, 'M').format('MMMM YYYY') %>  ➡️]]

- [[Yearly notes/<% date.format('YYYY') %>|<% date.format('YYYY') %>]]

## Monthly goals

- [ ] Task that will appear as a goal in the daily notes from <% date.format('MMMM YYYY') %>

