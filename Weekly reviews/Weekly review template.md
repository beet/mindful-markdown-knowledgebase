<%*
  // The note title will be _today's_ week, like "Weekly review 2023-W41"
  var weekString = tp.file.title.replace(/Weekly review /, '');
  var previousWeek = moment(weekString).subtract(1, 'week');
  var thisWeek = moment(weekString);
  var nextWeek = moment(weekString).add(1, 'week');
  var startDate = moment(weekString);
  var endDate = moment(weekString).add(5, 'd');
-%>
# Weekly review week <% thisWeek.format('WW') %>, <% startDate.format('YYYY-MM-DD') %> ~ <% endDate.format('YYYY-MM-DD') %>

- [[Monthly notes/<% thisWeek.format('YYYY-MM') %>|🗓️ Monthly notes - <% thisWeek.format('MMMM YYYY') %>]]
- [[Weekly reviews/Weekly review <% previousWeek.format('YYYY-[W]WW') %>|⬅️ Previous week's review]] | [[Weekly reviews/Weekly review <% nextWeek.format('YYYY-[W]WW') %>|Next week's review ➡️]]

## Previous week's reflection

- [[Issues.base]]
- [[Meetings.base]]
- [[Projects.base]]

> [!Note] Scratchpad:
> * Copy and paste the contents of the logbook from the following week below as a staging area
> * Move the bullet points down into the relevant sections:
>     * Select a line(s), and hit `SHIFT COMMAND + R` to select the section to move to.
>     * To de-duplicate project/issue/etc. links, select multiple lines and hit `SHIFT + COMMAND + D` 
> * Delete this callout when done


###  🏆 Wins


### 🧠 Learnings


### Projects


### Meetings


### Other


### Pressure

What did this week's _pressure_ feel like?

Pressure: 🟢 / 🟡 / 🔴

### Stress signals

(low overall goal count is a leading stress indicator, as are high counts of cancelled/forwarded goals)

- **✅ Completed goals:** 0
- **❌ Cancelled goals:** 0
- **↪ Forwarded goals:** 0
- **🧘‍♂️ Mindfulness goals:** 0
- **Context switching:** Y/N
- **Calendar blocking needed:** Y/N
- **Mental health days taken:** 0

## Goals

- Set your high-level goals after completing last week's reflection in [[Weekly notes/<% nextWeek.format('YYYY-[W]WW') %>|Weekly notes - week <% nextWeek.format('WW') %>]]
