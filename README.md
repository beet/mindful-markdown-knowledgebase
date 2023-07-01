# Mindful Markdown Knowledgebase

## Quick start

This will create the basic structure of notes that are tied together by a logbook:

- Clone this repo into a local dir

```
git clone git@github.com:beet/mindful-markdown-knowledgebase.git
```

- Open as a vault in Obsidian
  - Will probably need to enable community plugins and make sure the selected plugins are all installed
  - The system makes extensive use of the Calendar, Periodic Notes, Templater, and the almighty Tasks plugins. 
- Navigate to the [[Logbook]]
- Populate from template:
  - open the command palette with `COMMAND + P`, select "Templates: Insert template", and choose "Templates/Logbook template"

### Working with the log book

The [[Logbook]] is central to this system, and draws inspiration from [A Guide To Research Logbooks — Heloise F. Stevance](https://www.hfstevance.com/blog/logbooks). It is comprised of headings for year, month, and day, with each day being populated with a bullet point for each project/task being worked in, in a similar fashion to the [Bullet Journal](https://bulletjournal.com/) method, but in a single, flat file.

As I move from one task to the next throughout the day, I create a new bullet point and link to a page using action verbs like "Picking up", "Pushing on with", "Closing in", etc such as:

```markdown
* Wrapping up [[Project - Garden maintenance June 2023]]
* Picking up [[Project - Mindful Markdown Knowledgebase]]
* Updating [[Homebrew]]
* Merging in [[Ticket - All the bugs]]
```

Having a chronological log of past work helps me practice the [Bullet Journal Method](https://bulletjournal.com/pages/book):

> Track the past
> Order the present
> Design the future

This is achieved by logging the high-level projects & goals that I'm working on from moment-to-moment and day-to-day, reflecting on what I achieved from one week to the next, and from each month to the next, and steering them with purpose towards long-term goals.

#### Daily logging

As I start each new day, I insert a new heading for that day at the _top_ of that month _(in reverse chronological order)_ so I can quickly refer back to what I was working on during the previous days by scanning down the list from top to bottom and pick up where I left off.

- Can start a new day in the logbook by inserting the "Logbook template - new day" template:

```markdown
#### Sat 2023-07-01

- Started
```

#### Weekly review

On the first day of each week, I conduct a review of the previous week where I reflect on the work achieved, review any outstanding tasks, and in BuJu fashion re-schedule any that are still relevant, or cancel any that are not.

To conduct a weekly review:

- See [[README - Weekly reviews|Weekly reviews]]
- Start a new day in the logbook as above
- Insert the "Logbook template - new weekly review link" template
- Open the inserted link in a new tab, and follow the instructions

#### Monthly review

On the first day of each month, the first thing I do is conduct a [[README - Monthly reviews|monthly review]] of the previous month. When the first day of the month corresponds with the first day of the week, I'll complete the weekly review first.

Monthly reviews are really an opportunity to aggregate the weekly reviews together into flat lists that give a good bird's eye view of where time and energy went.

To start a new month in the logbook, insert the "Logbook template - new month" template:

```markdown
### July 2023

- [[Monthly notes/2023-07|July 2023]]

#### Sat 2023-07-01

- Started

```

To start a monthly review:

- Insert the "Logbook template - new monthly review link" template
- Open the link in a new tab, and follow the instructions
- I usually use the outline view of the logbook to browse back through the weekly reviews for the month and copy the log entries across to the monthly review
- Each monthly review is for the *previous* month, so the July monthly review would contain the June log entries

##### TIP: Archiving old months

Each monthly log can grow quite large, and I tend not to refer back further than the previous month after having completed review & reflection, so I typically create a logbook archive page, and move older months into it.

This helps reduce clutter, and makes the logbook page faster and more responsive to work with.

#### Yearly review

- Can start a new yearly review by inserting the "Logbook template - new yearly review" template into the logbook after starting a new day/month/year as per above
* Open the link in a new tab, and follow the instructions there

### Working with periodic notes

- [ ] TODO: flesh this out a bit with notes about the calendar, and how the daily/weekly/monthly notes and tasks are tied together

### Working with tasks

- [ ] TODO: flesh this out a bit with notes about how to schedule tasks, and how tasks in ad-hoc meeting notes will be picked up automatically

## Project pages

- [ ] TODO: create a `Projects/` folder with a default template, so you can just create new notes in there and have them populated automatically
  - Template for inserting links to the logbook
* Links to resources, like Github issue, related knowledge pages
* Their own detailed logbook
* Next actions at top
* Detailed notes separated by data
* Screenshots, code snippets, links, etc.

```markdown
---
tags:
  - issues
---
# Issue 1234 - Fix all the things

## Resources

* [Issue 1234](https://github.com/marketplacer/marketplacer/issues/1234)

## Logbook

* **22 Feb 2021:** start

## Next actions

- [ ] Do something

## Notes

All the things appear to be broken, need to fix them ASAP.

## 2021-02-22 - Digging deeper

Started looking into which things are broken,
confirmed that it's not all of them.
```

## Knowledge pages

* A page for each atomic unit of knowledge
* Back-links between related pages

```
Had to [[Restore sanitised DB snapshot]] then sort out [[Sorbet]] and move on to [[Deploying test sites]]
```

## Meeting notes

- [ ] TODO: create a dir for meeting notes with a default template and logbook link template
## Resources

* [Bullet Journal](https://bulletjournal.com/), a.k.a. BuJo, or BuJitsu
* [Getting Things Done - David Allen's GTD](https://gettingthingsdone.com/)
* [Zettelkasten - Wikipedia](https://en.wikipedia.org/wiki/Zettelkasten)
* [A guide to research logbooks - Heloise](https://hfstevance.com/blog/logbooks)
* [Obsidian](https://obsidian.md/)
