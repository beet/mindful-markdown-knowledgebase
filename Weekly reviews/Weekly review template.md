<%*
  var title = tp.file.title.replace(/Weekly review /, '');
  var startDate = moment(title);
  var endDate = moment(title).add(5, 'd'); // #add mutates the object
  var previousWeek = moment(title).subtract(1, 'week').format('YYYY-[W]WW');
-%>
# Weekly review <% startDate.format('YYYY-MM-DD') %> ~ <% endDate.format('YYYY-MM-DD') %>

## Previous week's reflection

* [[Projects]]
- [[Monthly notes/<% startDate.format('YYYY-MM') %>|Monthly notes - <% startDate.format('MMMM YYYY') %>]]
- [[Yearly notes/<% startDate.format('YYYY') %>|Yearly notes - <% startDate.format('YYYY') %>]]
- [[Weekly reviews/Weekly review <% previousWeek %>|Previous week's review]]

> [!Note] Scratchpad:
> * Copy and paste the contents of the logbook from the following week below as a staging area, and then move the bullet points down into the relevant sections.
> * Delete this and date headings when done.
> 



### Projects



### Meetings



### Other



## Goals

- Set your high-level goals after completing last week's reflection in [[Weekly notes/<% startDate.format('YYYY-[W]WW') %>|Weekly notes - week <% startDate.format('WW') %>]]
