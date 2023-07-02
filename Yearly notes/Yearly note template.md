<%* var date = moment(tp.file.title); -%>
# <% date.format('YYYY') %>

[[Yearly notes/<% moment(tp.file.title).subtract(1, 'y').format('YYYY') %>|⬅️ <% moment(tp.file.title).subtract(1, 'y').format('YYYY') %>]] | [[Yearly notes/<% moment(tp.file.title).add(1, 'y').format('YYYY') %>|<% moment(tp.file.title).add(1, 'y').format('YYYY') %> ➡️]]

## Goals

- Add your yearly goals here

### Do more of

- Foo

### Do less of

- Bar

## Future log

### January <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-01|<% date.format('MMMM YYYY') %>]]

### February <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-02|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### March <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-03|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### April <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-04|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### May <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-05|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### June <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-06|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### July <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-07|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### August <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-08|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### September <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-09|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### October <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-10|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### November <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-11|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### December <% date.format('YYYY') %>

- [[Monthly notes/<% date.format('YYYY') %>-12|<% date.add(1, 'M').format('MMMM YYYY') %>]]

