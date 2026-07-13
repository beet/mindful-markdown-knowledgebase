# Claude Code Instructions for Obsidian Vault

## Obsidian CLI

All vault interactions must use the `obsidian` CLI (`/usr/local/bin/obsidian`) rather than direct file operations where possible. The CLI communicates with the running Obsidian app and respects vault indexing, links, and plugins.

### Key syntax rules

- Options use `key=value` format (no dashes): `obsidian read file="My Note"`
- `file=<name>` resolves by name (like wikilinks — no path needed)
- `path=<path>` is exact: `folder/note.md`
- Quote values containing spaces: `name="My Note"`
- Use `\n` for newlines and `\t` for tabs in content values
- Target a specific vault: `obsidian vault=<name> <command>`

### Common commands

```bash
# Read a file
obsidian read file="Note Name"
obsidian read path="Daily notes/2026-03-26.md"

# Create a file
obsidian create name="New Note" content="# Heading\nContent here"
obsidian create path="Project notes/new-project.md" template="Project note template"

# Append / prepend content
obsidian append file="Note Name" content="New paragraph"
obsidian prepend file="Note Name" content="Intro text"

# Search the vault
obsidian search query="search term"
obsidian search query="search term" path="Daily notes"
obsidian search:context query="search term"

# List files / folders
obsidian files
obsidian files folder="Daily notes" ext=md
obsidian folders

# Properties (frontmatter)
obsidian property:read name="status" file="Note Name"
obsidian property:set name="status" value="done" file="Note Name"
obsidian properties file="Note Name"

# Tags
obsidian tags
obsidian tags file="Note Name"

# Tasks
obsidian tasks todo
obsidian tasks file="Note Name"
obsidian task path="Daily notes/2026-03-26.md" line=12 toggle   # toggle/done/todo are flags, not subcommands
obsidian task ref="Daily notes/2026-03-26.md:12" done           # ref=<path:line> shorthand

# Daily note
obsidian daily:read
obsidian daily:append content="- [ ] New task"

# Move / rename / delete
obsidian move file="Note Name" to="New Folder"
obsidian rename file="Note Name" name="Better Name"
obsidian delete file="Note Name"

# Links
obsidian links file="Note Name"
obsidian backlinks file="Note Name"

# Vault info
obsidian vault
obsidian files total

# Headings, templates, commands
obsidian outline file="Note Name"                  # list headings (format=tree|md|json)
obsidian templates                                  # list available templates
obsidian template:read name="Project note template"
obsidian template:insert name="Project note template"
obsidian commands filter=workspace                  # list Obsidian commands
obsidian command id=editor:toggle-source            # run an Obsidian command

# Bookmarks, recents, random
obsidian bookmarks
obsidian bookmark file="Note Name"
obsidian recents
obsidian random:read folder="Resources"

# Vault health
obsidian unresolved      # links pointing to nonexistent notes
obsidian orphans         # notes with no incoming links
obsidian deadends        # notes with no outgoing links
obsidian aliases
obsidian wordcount file="Note Name"

# Bases (database views)
obsidian bases
obsidian base:views file="Base Name"
obsidian base:query file="Base Name" view="View Name" format=json
```

### When to use the CLI vs direct file tools

| Task                              | Use                                                   |
| --------------------------------- | ----------------------------------------------------- |
| Read note content                 | `obsidian read`                                       |
| Create a note                     | `obsidian create`                                     |
| Append/prepend to a note          | `obsidian append` / `obsidian prepend`                |
| Search vault content              | `obsidian search`                                     |
| Read/write frontmatter properties | `obsidian property:read` / `obsidian property:set`    |
| List files, tags, tasks           | `obsidian files` / `obsidian tags` / `obsidian tasks` |
| Move or rename a file             | `obsidian move` / `obsidian rename`                   |
| Read `.obsidian/` config files    | Direct `Read` tool (CLI doesn't expose these)         |
| Edit templates or CSS snippets    | Direct `Edit` tool (no CLI equivalent)                |
| Git operations                    | `Bash` with git commands                              |

### Output formats

Many list commands support `format=json|tsv|csv` for structured output. Not all commands accept `format=` (e.g. `files` does not), so check `obsidian help <command>` first. Note that `tasks` defaults to `text`, not `tsv`.

```bash
obsidian tags counts format=json
obsidian tasks todo format=json
obsidian backlinks file="Note Name" format=json
obsidian base:query file="Base Name" view="View Name" format=json
```

### Getting help

```bash
obsidian --help              # Full command reference
obsidian help <command>      # Help for a specific command (e.g. obsidian help search)
```

## Folder Structure

* Attachments/ - Binary files like screenshots, PDFs, etc.
* Daily notes/ - Todos and logbook for each day's work
* Issue notes/ - Support tickets that have been worked on, including tasks, logbook, and notes.
* Meeting notes/ - Tasks and notes taken during meetings
* Monthly notes/ - Aspirational goals for the month
* Monthly reviews/ - Review of that month's projects, meetings, and other activities, with links to the corresponding weekly notes, and sometimes a summary
* Project notes/ - Resources, tasks, logbook, and notes for a project
* Resources/ - Each page is a note about a self-contained resource or piece of information
* Weekly notes/ - Aspirational goals for the week
* Weekly reviews/ - Lists of projects, meetings, and other activities that were worked on this week
* Yearly notes/ - Aspirational goals for the year, and links to monthly notes
* Yearly reviews/ - Links to monthly reviews from the year, summaries of positive and negative things from the year
- Diagrams/ - Usually Mermaid diagrams like ERDs, UML sequence, state machines, etc.

## Markdown formatting

- Headings should be followed by a blank line
- When generating Markdown to append to an existing page, it will have a H1 heading for the title, and typically a H2 heading for notes, generated headings should start from H3
