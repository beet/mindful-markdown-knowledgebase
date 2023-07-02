<%* var date = moment(tp.file.title); -%>
# Week <% date.format('W, MMMM YYYY') %>

[[Weekly notes/<% moment(tp.file.title).subtract(1, 'w').format('YYYY-[W]WW') %>|⬅️ Week <% moment(tp.file.title).subtract(1, 'w').format('WW') %>]] | [[Weekly notes/<% moment(tp.file.title).add(1, 'w').format('YYYY-[W]WW') %>|Week <% moment(tp.file.title).add(1, 'w').format('WW') %> ➡️]]

- [[Monthly notes/<% date.format('YYYY-MM') %>|<% date.format('MMMM YYYY') %>]]

## Weekly goals

- [ ] Task that will appear as a goal in the daily notes from week <% date.format('WW') %>
