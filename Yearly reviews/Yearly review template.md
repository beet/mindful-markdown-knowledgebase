<%*
  var date = moment(tp.file.title);
  var year = date.format('YYYY');
  var prevDate = moment(tp.file.title).subtract(1, 'year');
  var prevYear = prevDate.format('YYYY');
-%>
# Yearly review of <% prevYear %>

## Reflection

See [Forget New Year's Resolutions and Conduct a 'Past Year Review' Instead – The Blog of Author Tim Ferriss](https://tim.blog/2018/12/28/past-year-review/)

- [[Monthly notes/<% prevDate.format('YYYY') %>-01|<% prevDate.format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-02|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-03|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-04|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-05|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-06|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-07|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-08|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-09|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-10|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-11|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]
- [[Monthly notes/<% prevDate.format('YYYY') %>-12|<% prevDate.add(1, 'M').format('MMMM YYYY') %>]]

### Positive things

- Create an objective list of things that elicited a positive emotion

### Negative things

- It's often surprising how few negative things there actually were

## Goals

- Set your goals for the year in [[Yearly notes/<% year %>|<% year %>]]
