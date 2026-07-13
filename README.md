# Mindful Markdown Knowledgebase

This is an [Obsidian](https://obsidian.md/) template vault designed to provide a task management and Personal Knowledge Management (PKM) system that draws inspiration from the [Bullet Journal](https://bulletjournal.com/) method and [research logbooks](https://www.hfstevance.com/blog/logbooks).

## Quick start

Clone this repo into a local dir:

```
git clone git@github.com:beet/mindful-markdown-knowledgebase.git
```

- Open as a vault in Obsidian
-  Enable community plugins and install and enable the plugins below
- Reload Obsidian, then go to today's daily note with `COMMAND + T`, and it should be populated from a template

### Plugins

Plugins to install and enable: _(the links will open Obsidian's plugin page for each, can install and enable from there, some will already have pre-configured settings and hotkeys from the template vault)_

- [ ] [Calendar](obsidian://show-plugin?id=calendar)
- [ ] [Coloured Tags Wrangler](obsidian://show-plugin?id=colored-tags-wrangler) - optional, if you use tags like #DONE
- [ ] [Minimal Theme Settings](obsidian://show-plugin?id=obsidian-minimal-settings) - optional
- [ ] [Page Heading From Links](obsidian://show-plugin?id=page-heading-from-links), or an equivalent
- [ ] [Periodic Notes](obsidian://show-plugin?id=periodic-notes)
- [ ] [QuickAdd](obsidian://show-plugin?id=quickadd)
- [ ] [Quick Switcher++](obsidian://show-plugin?id=darlal-switcher-plus) - optional, can hit `COMMAND + R` to navigate the page by heading
- [ ] [Rapid Notes](obsidian://show-plugin?id=obsidian-rapid-notes)
- [ ] [Style Settings](obsidian://show-plugin?id=obsidian-style-settings) - optional
- [ ] [Tasks](obsidian://show-plugin?id=obsidian-tasks-plugin)
- [ ] [Templater](obsidian://show-plugin?id=templater-obsidian)
- [ ] [Widgets](obsidian://show-plugin?id=widgets) - optional, if you want to show a clock in the sidebar

Some will already have settings saved in this template vault that will come into effect, like the Quick Add macros.

## Working with daily notes

Daily logging is central to this system, and draws inspiration from [A Guide To Research Logbooks — Heloise F. Stevance](https://www.hfstevance.com/blog/logbooks).

It begins with the core **Daily Notes** plugin, and relies heavily on the **[Periodic Notes](https://github.com/liamcain/obsidian-periodic-notes)** plugin to provide weekly, monthly, and yearly notes, with the [Templater](https://github.com/SilentVoid13/Templater) plugin populating notes from templates as they are created automatically on the fly.

Navigating to today's [[README - Daily notes|daily note]] with a hotkey like COMMAND/CONTROL+T or the sidebar calendar will create a new daily note under the `Daily notes/` folder, that will be pre-populated with content from a template:

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

### Daily logging

As I move from one task to the next throughout the day, I create a new bullet point in the **Log** section at the bottom of today's daily note with a link to a project page or meeting note using action verbs like "Picking up", "Pushing on with", "Closing in", etc such as:

```markdown
* Wrapping up [[Project - Garden maintenance June 2023]]
* Picking up [[Project - Mindful Markdown Knowledgebase]]
* Updating [[Homebrew]]
* Merging in [[Ticket - All the bugs]]
* [[Meeting notes/Meeting 2024-03-09 - Sprint planning|Meeting 2024-03-09 - Sprint planning]]
```

This helps pick up where I left off, and also drives the weekly review.

#### QuickAdd macros

I've defined QuickAdd macros to tie everything together. The workflow is to use QuickAdd to append a wiki-link to the logbok section of today's daily note, position the cursor in it and hit `COMMAND + SHIFT + N` to open it, and Templater will populate it from a template.

Bring up the **command pallette** and type "qa" to filter by QuickAdd choices, then select from one of the following:

* **QuickAdd: Issue link**
    * From the **daily note**, will prompt for the issue no. and append a link to the bottom of the page
* **QuickAdd: Meeting link**
    * From the **daily note**, will prompt for a meeting title and append a link to the bottom of the page
* **QuickAdd: Project link**
    * From any page, will prompt for a project title and append a link to the bottom of the page
* **QuickAdd: Logbook entry**
    * From a **project page**, will prompt for a logbook entry and insert a date-stamped entry into its logbook section
* **QuickAdd: Quick task: today**
    * From any page, will prompt for a task and add it to today's daily note for rapid capture without context switching
* **QuickAdd: Quick task: current file**
    * From a **project page**, will prompt for a task and add it to the project's todos, for rapid capture without jumping up to the top of the page
* **QuickAdd: Weekly review link**
    * From today's daily note, appends a link to this week's weekly review to the bottom of the page
* **QuickAdd: Monthly review link**
    * From today's daily note, appends a link to this month's monthly review to the bottom of the page
* **QuickAdd: Yearly review link**
    * From today's daily note, appends a link to this year's yearly review to the bottom of the page

## Weekly review

On the first day of each week, I conduct a review of the previous week where I reflect on the work achieved, review any outstanding tasks, and in BuJu fashion re-schedule any that are still relevant, or cancel any that are not.

To conduct a [[README - Weekly reviews|weekly review]]:

- Open today's daily note and use the QuickAdd macros to insert a weekly review link, position the cursor in it and hit `OPT + COMMAND + N` to open it and populate from a template.
- Open the inserted link in a new tab, and follow the instructions
- The weekly review page includes a link to create a weekly note page, where I set goals for the week which will automatically appear in daily notes for that week

### Weekly notes

The [[README - Weekly notes|weekly notes]] are where I set high-level goals for the week. The weekly goals appear in the dashboard for each daily note of that week, and are aggregated into the monthly notes page for a future log of upcoming intentions.

It shows any tasks scheduled for the week, and the monthly goals from the monthly notes page.

## Monthly review

On the first day of each month, the first thing I do is conduct a [[README - Monthly reviews|monthly review]] of the previous month. When the first day of the month corresponds with the first day of the week, I'll complete the weekly review first.

Monthly reviews are really an opportunity to aggregate the weekly reviews together into flat lists that give a good bird's eye view of where time and energy went.

To start a monthly review:

- Open today's daily note and use the QuickAdd macros to insert a monthly review link, position the cursor in it and hit `OPT + COMMAND + N` to open it and populate from a template.
- Open the link in a new tab, and follow the instructions
- Each monthly review is for the *previous* month, so the July monthly review would contain the June log entries
- The monthly review pages includes a link to create a [[README - Monthly notes|monthly note]] page where I set goals for the month which will apppear in weekly notes for that month

### Monthly notes

The [[README - Monthly notes|monthly notes]] page is where I set high-level goals for the month, which are aggregated into the yearly notes page.

It shows all scheduled tasks for the month, and aggregates the weekly goals into a future log of intentions.

## Yearly review

To start a new [[README - Yearly reviews|yearly review]]:

- Open today's daily note and use the QuickAdd macros to insert a yearly review link, position the cursor in it and hit `OPT + COMMAND + N` to open it and populate from a template.
* Open the link in a new tab, and follow the instructions there
* It includes a link to create a [[README - Yearly notes|yearly note]], with a section to set goals for the year, and a future log that aggregates goals from the year's monthly notes

### Yealy notes

The [[README - Yearly notes|yearly notes]] provide a section to intentionally plan to do more of the things that elicited a positive response from the previous year, and less of the things that were negative.

It also creates a **future log** that aggregates the goals from the monthly notes for the year.

## Working with tasks

The mighty [Obsidian Tasks](https://github.com/obsidian-tasks-group/obsidian-tasks) plugin provides the basis for managing tasks.

Any task anywhere on any page with a **due date** will appear on that date's daily note as either due or overdue.

* Tasks in daily notes and meeting notes _(or any note with an ISO8601 date in the filename)_ don't need a due date to be explicitly assigned.

### Tasks in daily notes

Any todo in a daily note is scheduled on that day, and will appear in the various tasks lists.

- The [[README - Daily notes|daily note template]] shows all tasks from all pages that are due on that day
- It also shows any tasks that are overdue, so you never have to worry about forgetting anything

You can actually add a due date to a task in a daily note to schedule it on a different date.

### Tasks in project pages

The [[README - Project notes|project notes template]]  has a section at the top that shows all tasks that are due today and overdue from anywhere on that page.

It provides a **Next actions** section for defining high-level tasks to move the project forward, which can be given a date when time sensitive.

I quite often create low-level ad-hoc todo lists as I'm working, which can also be given due dates as needed.

Any tasks in any project page with a due date will appear in the daily note for that day.

### Tasks in meeting notes

The Tasks plugin has the option to [use the filename as the scheduled date for undated tasks](https://publish.obsidian.md/tasks/Getting+Started/Use+Filename+as+Default+Date), which when enabled means that any tasks added to meeting notes, which follow the filename convention of "Meeting YYYY-MM-DD - Title", will automatically appear in the daily note for that date.

This allows for rapid logging of action items during meetings, with confidence that they will float up in the daily notes and not be forgotten.

## Project notes

**Project notes** are open-ended documents that are longer-lived, often span multiple issues, and are more about sustained context than a discrete deliverable. They become a living document that may reference many other resources and issues underneath it.

When creating new project notes, they will be populated from a Templater template that provides several sections:

* **Resources:** Links to resources like Github issues, related knowledge pages, etc.
* **Today/overdue tasks:** Dashboard summarising tasks due today, and overdue tasks from anywhere within the project page
* **Logbook:** Each project page keeps its own detailed logbook summarising changes made each day
* **TODOs:** Next actions at the top of the page
* **Notes:** Detailed notes separated by date-stamped headings for each day of work on the project

## Issue notes

**Issue notes** are ticket-scoped — they have an ID, a defined start and end, and tend to be reactive (support issues, bugs, specific tasks). They're queryable by ticket prefix and map 1:1 to external systems.

When creating new issues notes, they will also be populated from a Templater template that provides a very similar structure to project notes.

## Knowledge/fleeting pages

* Pretty much everything else goes in the **Resources** folder.
* A page for each atomic unit of knowledge
* Back-links between related pages

```Markdown
Had to [[Restore sanitised DB snapshot]] then sort out [[Sorbet]] and move on to [[Deploying test sites]]
```

## Meeting notes

* Note that any tasks that are added to meeting notes are automatically treated as being scheduled for that day, and will appear in the daily notes.

## Resources

* [Obsidian](https://obsidian.md/)
* [Bullet Journal](https://bulletjournal.com/), a.k.a. BuJo, or BuJitsu. A "mindfulness practice disguised as a productivity system".
* [A guide to research logbooks - Heloise](https://hfstevance.com/blog/logbooks)

## What I've learned about myself through reflection and review

Creating a well structured knowledge base yields the most value when incorporated with a review/reflection process. I've adapted a system that's inspired by the Bullet Journal process, comprised of weekly/monthly/yearly reviews, and weekly/monthly/yearly goals.

It turns out that structuring them this way is conducive to performing _sentiment analysis_ with AI.

### What Claude knows about me that I don't

Asked Claude "What do you know about me that I don't?", and it said:

**Your stress has a very predictable signature**

When things get hard, *mindfulness goals* appear in your weekly notes — *"bring my best self"*, *"act well in your given role"*, *"remain in harmony with the nature of all things"*. When those goals start getting cancelled or forwarded rather than ticked off, that's the canary. It happened in many weeks. You're essentially logging your own stress response without labelling it as such.

**You absorb more than you let on**

A comment was off-hand enough that it probably wasn't intended as a serious criticism — but you logged it, quoted it, reacted to it in writing, and then literally wrote *"do NOT try to drive outcomes!!!"* into your weekly goals the following week. That's not someone who lets things wash over them.

**You do your best work when left alone**

The Aug–Nov 2025 run was your most sustained positive stretch of the year — 14 weeks. What characterised it? A focused project, fewer meetings, and no major fires. The contrast with July (44 meetings, daily huddles) is stark.

**The long-running project is a proxy for something bigger**

It's been deferred, parked, rekindled, and pushed aside more times than any other piece of work. But you keep coming back to it. It's clearly something you care about — the backtesting, the algorithm design, the careful notes — and it keeps getting deprioritised by things that feel less important. That probably stings more than you've written down.

### Incorporating stress signal indicators into reviews

**Simplest — tag your mindfulness goals**

When you write a mindfulness goal (like "bring my best self" / "remain in harmony with the nature of all things"), add a  tag inline. Over time you'd be able to search for these and see the clusters without any extra effort — you're already writing them, just making them queryable.

**Weekly — add a one-line mood/pressure rating**

At the top of each weekly note, a simple line like:

```
Pressure: 🟢 / 🟡 / 🔴
```

Low friction, no prose required, and something Claude (or you) could query across weeks to plot trends. Would have made the July 2025 trough immediately visible in the data.

**Monthly reviews — add a "stress signals" section**

A small structured section that prompts you to look back explicitly:

```markdown
Stress signals this month

- Mindfulness goals: cancelled / forwarded / completed
- Mental health days taken:
- Calendar blocking needed: y/n
- Weeks where goals were sparse (1 or fewer):
```

Takes two minutes to fill in but creates a longitudinal record you can actually reason about.

**Yearly reviews — a "cost of the year" reflection**

You already do wins/learnings — a third lens of *"what did this year cost me?"* alongside the positives would surface the through-lines that are currently only visible in retrospect (like the 2025 leaving arc). Something like:

```markdown
What this year cost

- Periods of sustained stress and why
- Things I kept absorbing that I shouldn't have
- What I wish I'd noticed sooner
```

**Longer term — a dedicated wellbeing note**

A single living Resource note (safe to keep private) that you update periodically with patterns you've noticed. A place to collect the signals so they don't just live buried in daily notes. Something like .

The common thread across all of these: you're already generating the signal, you're just not labelling it in a way that makes it easy to see from a distance. The goal would be to make the invisible visible without adding much overhead.

### Could mindfulness goals be stress indicators?

*Could the presence of mindful goals be a leading indicator, while cancelled/forwarded mindfulness goals are a red flag?*

Yes, almost certainly — and the data supports it:

**Leading indicator** — a mindfulness goal appearing signals that something is already creating friction. By the time you're writing "rise above Foo" or "bring my best self to Bar", the pressure is already there. It's not a prediction, it's an early acknowledgement that you're having to consciously manage your response to something.

**Red flag** — when those goals then get cancelled or forwarded, it means the friction has won. You set the intention and couldn't even hold onto it. W10 Mar 2026 is the clearest example — the mindfulness goal itself got cancelled, right as fires were peaking.

**The progression looks something like:**

```
Normal goals → Mindfulness goal appears (pressure building)
             → Mindfulness goal completed (holding steady)
             → Mindfulness goal forwarded (slipping)
             → Mindfulness goal cancelled (overwhelmed)
             → Sparse goals / single vague goal (survival mode)
```

W31–W32 July 2025 is a good example of the full arc compressed into two weeks — the "do NOT try to drive outcomes!!!" goal appeared and was completed, but only because the month was already in freefall.

The interesting implication: if you'd been tracking this in real time, a forwarded mindfulness goal would have been a signal to intervene — reduce commitments, push back on meetings, protect focus time — *before* hitting the cancelled/survival mode stage.

### Goals set per week 

- **Low goal count (1) is a reliable stress signal** — W19, W28, W32, W42, W46, W50, W52, W02, W09 all sit at 1, and most of those align with either crisis periods or deliberate wind-down
- **High goal count (6–7) signals energy and engagement** — W14, W15, W35, W36 were all relatively positive, focused weeks
- **The Jul–Aug 2025 trough is visible** — W28–W32 dips to 1–2 goals and stays there
- **Goal count alone is a decent proxy for how you're feeling**, even before looking at the content

### Leading indicators of rising stress

*So if I track completed/cancelled/forwarded goals, as well as the no. of goals, and the presence of mindfulness goals, I should have a pretty good leading indicator of rising stress?*

Yes — and those four signals complement each other well:

**Goal count** — the broadest signal. Dropping below 2-3 suggests bandwidth is already constrained, even before you look at content.

**Mindfulness goal present** — confirms it's not just a quiet week. You're consciously managing your response to something.

**Forwarded goals** — the earliest actionable warning. You still had the intention but lost the capacity to execute. This is where intervention is most useful — you're not overwhelmed yet.

**Cancelled goals** — the lagging confirmation. By this point the stress has already peaked. Useful for retrospection but too late to act on.

Together they form a rough progression:

```
↓ Goal count
  → Mindfulness goal appears        = pressure acknowledged
    → Goals start forwarding        = capacity slipping  ⚠️ act here
      → Goals get cancelled         = overwhelmed
        → Single vague goal / none  = survival mode
```

The one caveat worth noting: **social events and leave days inflate the goal count and completion rate** without reflecting real productive capacity. A week with 4 goals that are all boat days and long weekends looks healthy but isn't the same as 4 substantive work goals all ticked off.

So a refined version might weight goals by type — aspirational/work goals vs. calendar anchors — to get a cleaner signal. Though that adds friction, which defeats the purpose if it stops you doing it consistently.

The simplest version that would actually work: at the end of each weekly note, one line —

```
Pressure: 🟢  Goals: 5  ↪ 0  ❌ 0  🧘 n
```

Queryable, low friction, and honest.

---

## Next actions

- [x] Maybe re-organise things with the PARA system?
- [ ] Maybe consolidate issues with projects, and just use project pages for everything?
- [ ] Tweak the .gitignore like [Allow only some files in subdirectories with .gitignore - Stack Overflow](https://stackoverflow.com/questions/16313432/allow-only-some-files-in-subdirectories-with-gitignore) to exclude the user generated files
- [ ] Move the recurring tasks out to their own files within their folders, and add them to .gitignore so the recursions don't clog things up
