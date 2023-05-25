# Mindful Markdown Knowledgebase

**Disclaimer:** I'm by no means an expert, our brains are all different, what works for me may not work for you.

As Chef John would say, it's just a *technique*, not a recipe to follow to the letter.

## Work smarter, not harder

* **DRY:** write once, recall often
* **Context switching:** should be avoided, but is inevitable, so make it less painful
* **Peace of mind!** 😀

## The system

* Mindful
* Markdown
* Knowledge Management

### Mindful

Borrows elements of reflection and review from **Bullet Journalling**

* Less about doing more things
* More about being more effective
* Paradoxically, gets more done

#### Slow is the new fast

> Occasionally you need to waste time for a while to be able to spend it better later. If you’re constantly busy, busy, busy, you don’t have any headspace to reflect on where every daily step is ultimately leading you. Running real fast is no good if it’s into a brick wall.

DHH, [Getting less done](https://m.signalvnoise.com/getting-less-done/)

## Markdown

Plain-text in all the places, forever

* Unstructured data accommodates any system
* Portable, extensible
* Timeless

## Knowledge management

A system for _finding_ information, not just filing it away.

> The mind is for having ideas, not holding them

David Allen, creator of Getting Things Done (GTD)

### Pareto's principle

The 20% of things I need to refer to regularly to do 80% of my work.

## The Process

![[Plan Act Log Reflect(2).png]]

### Reflect & plan

Borrows elements from research logbooks

* Driven by logbook
* Weekly & monthly reviews
* Sets goals for each week/month

> There is nothing so useless as doing efficiently that which should not be done at all

Peter Drucker

### Act & log

* **Logbook:** an entry for each thing worked on each day
* **Project pages:** a page for each thing being worked on
* **Knowledge pages:** a page for anything I need to refer back to more than once

> The only difference between science, and screwing around, is writing things down

Adam Savage, on the origin of "I reject your reality, and substitute my own"

## The logbook

* Headings for year, month, and day
* Actions like "pick up", "push on", "merge in", "paired up"
* Links to pages for each thing

---

```markdown
# Logbook

## Feb 2021

### Mon 2021-02-22

* Picked up [[Issue 1234 - Fix all the things]]
* [[Meeting 2021-02-22 - Backend working group]]

### Tue 2021-02-23

* Pushing on with [[Issue 1234 - Fix all the things]]
* Polished off [[Issue 2345 - Error on checkout]]
```

## Project pages

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


> Had to `[[Restore sanitised DB snapshot]]` then sort out `[[Sorbet]]` and move on to `[[Deploying test sites]]`


## Resources

* [Bullet Journal](https://bulletjournal.com/), a.k.a. BuJo, or BuJitsu
* [Getting Things Done - David Allen's GTD](https://gettingthingsdone.com/)
* [Zettelkasten - Wikipedia](https://en.wikipedia.org/wiki/Zettelkasten)
* [A guide to research logbooks - Heloise](https://hfstevance.com/blog/logbooks)
* [Obsidian](https://obsidian.md/)
