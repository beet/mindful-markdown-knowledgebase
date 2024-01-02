# Mindful Markdown Knowledgebase

This is an Obsidian template vault designed to provide a task management and Personal Knowledge Management, PKM, system that draws inspiration from the [Bullet Journal](https://bulletjournal.com/) method and [research logbooks](https://www.hfstevance.com/blog/logbooks).

## Quick start

This will create the basic structure of notes that are tied together by a logbook:

- Clone this repo into a local dir

```
git clone git@github.com:beet/mindful-markdown-knowledgebase.git
```

- Open as a vault in Obsidian
  - Will probably need to enable community plugins and make sure the selected plugins are all installed
  - The system makes extensive use of the Calendar, Periodic Notes, Templater, and the almighty Tasks plugins. 
- After enabling the Daily Notes plugin, go to today's daily note, and it should be populated from a template

### Working with daily notes

Daily logging is central to this system, and draws inspiration from [A Guide To Research Logbooks — Heloise F. Stevance](https://www.hfstevance.com/blog/logbooks).

It begins with the core **Daily Notes** plugin, and relies heavily on the **[Periodic Notes](https://github.com/liamcain/obsidian-periodic-notes)** plugin to provide weekly, monthly, and yearly notes, with the [Templater](https://github.com/SilentVoid13/Templater) plugin populating notes from templates as they are created automatically on the fly.

Navigating to today's daily note with a hotkey or the sidebar calendar will create a new daily note under the `Daily notes/` folder, that will be pre-populated with content from a template:

* Navigation links to the prev/next daily note
* Tasks due/completed today
* Overdue tasks
* Upcoming tasks this week
* This week's goals
* Today's tasks
* Today's **log**


Having a chronological log of past work helps me practice the [Bullet Journal Method](https://bulletjournal.com/pages/book):

> Track the past,
> Order the present,
> Design the future

This is achieved by logging the high-level projects & goals that I'm working on from moment-to-moment and day-to-day, reflecting on what I achieved from one week to the next, and from each month to the next, and steering them with purpose towards long-term goals.

#### Daily logging

As I move from one task to the next throughout the day, I create a new bullet point in the **Log** section at the bottom of today's daily note with a link to a project page using action verbs like "Picking up", "Pushing on with", "Closing in", etc such as:

```markdown
* Wrapping up [[Project - Garden maintenance June 2023]]
* Picking up [[Project - Mindful Markdown Knowledgebase]]
* Updating [[Homebrew]]
* Merging in [[Ticket - All the bugs]]
```

This helps pick up where I left off, and also drives the weekly review.

#### Weekly review

On the first day of each week, I conduct a review of the previous week where I reflect on the work achieved, review any outstanding tasks, and in BuJu fashion re-schedule any that are still relevant, or cancel any that are not.

To conduct a weekly review:

- See [[README - Weekly reviews|Weekly reviews]]
- Insert the "Logbook template - new weekly review link" template
- Open the inserted link in a new tab, and follow the instructions
- The weekly review page includes a link to create a weekly note page, where I set goals for the week which will automatically appear in daily notes for that week

##### Weekly notes

The weekly notes is where I set high-level goals for the week, which are aggregated into the monthly notes page.

It shows any tasks scheduled for the week, and the monthly goals from the montly notes page.

#### Monthly review

On the first day of each month, the first thing I do is conduct a [[README - Monthly reviews|monthly review]] of the previous month. When the first day of the month corresponds with the first day of the week, I'll complete the weekly review first.

Monthly reviews are really an opportunity to aggregate the weekly reviews together into flat lists that give a good bird's eye view of where time and energy went.

To start a monthly review:

- Insert the "Logbook template - new monthly review link" template
- Open the link in a new tab, and follow the instructions
- Each monthly review is for the *previous* month, so the July monthly review would contain the June log entries
- The monthly review pages includes a link to create a monthly note page where I set goals for the month which will apppear in weekly notes for that month

##### Monthly notes

The monthly notes page is where I set high-level goals for the month, which are aggregated into the yearly notes page.

It shows all scheduled tasks for the month, and aggregates the weekly goals.

#### Yearly review

- Can start a new yearly review by inserting the "Logbook template - new yearly review" template into the logbook after starting a new day/month/year as per above
* Open the link in a new tab, and follow the instructions there
* It includes a link to create a yearly note, with a section to set goals for the year, and a future log that aggregates goals from the year's monthly notes

##### Yealy notes

The yearly notes provide a section to intentionally plan to more more of the things that elicited a positive response from the previous year, and less of the things that were negative.

It also creates a **future log** that aggregates the goals from the monthly notes for the year.

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
* Note that any tasks that are added to meeting notes are automatically treated as being scheduled for that day, and will appear in the daily notes.

## Resources

* [Obsidian](https://obsidian.md/)
* [Bullet Journal](https://bulletjournal.com/), a.k.a. BuJo, or BuJitsu. A "mindfulness practice disguised as a productivity system".
* [A guide to research logbooks - Heloise](https://hfstevance.com/blog/logbooks)
