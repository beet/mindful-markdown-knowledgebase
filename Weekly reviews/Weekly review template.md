<%*
  // The note title will be _today's_ week, like "Weekly review 2023-W41"
  var weekString = tp.file.title.replace(/Weekly review /, '');
  var thisWeek = moment(weekString);
  var nextWeek = moment(weekString).add(1, 'week');
  var startDate = moment(weekString).subtract(1, 'week');
  var endDate = moment(weekString).subtract(1, 'week').add(5, 'd'); // #add and #subtract mutate the object
-%>
# Weekly review week <% thisWeek.format('WW') + ', ' + startDate.format('YYYY-MM-DD') %> ~ <% endDate.format('YYYY-MM-DD') %>

- [[Monthly notes/<% thisWeek.format('YYYY-MM') %>|🗓️ Monthly notes - <% thisWeek.format('MMMM YYYY') %>]]
- [[Weekly reviews/Weekly review <% startDate.format('YYYY-[W]WW') %>|⬅️ Previous week's review]] | [[Weekly reviews/Weekly review <% nextWeek.format('YYYY-[W]WW') %>|Next week's review ➡️]]

## Previous week's reflection

- **🏆 WINS:** 
- **🧠 LEARNINGS:** 

> [!Note] Scratchpad:
> * Copy and paste the contents of the logbook from the following week below as a staging area, and then move the bullet points down into the relevant sections.
> * Delete this callout when done
> 



### Projects


### Meetings


### Other


## Goals

- Set your high-level goals after completing last week's reflection in this week's [[Weekly notes/<% thisWeek.format('YYYY-[W]WW') %>|Weekly notes - week <% thisWeek.format('WW') %>]]
