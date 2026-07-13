<%*
  var date = moment(tp.file.title);
  var year = date.format('YYYY');
  var nextYear = moment(tp.file.title).add(1, 'year').format('YYYY');
  // var prevDate = moment(tp.file.title).subtract(1, 'year');
  // var prevYear = prevDate.format('YYYY');
-%>
# Yearly review of <% year %>

## Reflection

See [Forget New Year's Resolutions and Conduct a 'Past Year Review' Instead – The Blog of Author Tim Ferriss](https://tim.blog/2018/12/28/past-year-review/)

- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-01|<% date.format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-02|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-03|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-04|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-05|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-06|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-07|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-08|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-09|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-10|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-11|<% date.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly reviews/Monthly review <% date.format('YYYY') %>-12|<% date.add(1, 'M').format('MMMM YYYY') %>]]

### Positive things

- Create an objective list of things that elicited a positive emotion

### Negative things

- It's often surprising how few negative things there actually were

### Pressure

* How did weekly/monthly pressure track over the year?

### Stress signals

- How did weekly/monthly stress signals track over the year?

## Goals

- Set your goals for the coming year in [[Yearly notes/<% nextYear %>|<% nextYear %>]]
