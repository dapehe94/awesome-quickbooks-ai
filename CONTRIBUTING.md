# Contributing

Thanks for helping keep this list useful. Pull requests and issues are both fine; an issue with a link is enough if
you would rather not open a pull request.

## Inclusion criteria

An entry belongs here if it is:

1. **About QuickBooks.** Built for QuickBooks Desktop (Pro, Premier, Enterprise), QuickBooks Online or QuickBooks
   Time. Tools for many accounting systems are welcome when QuickBooks is one of them.
2. **AI-related, or a building block for it.** An agent skill or plugin, an MCP server, an agent, a CLI an agent can
   drive, a starter kit, a hosted AI or API service, or a library that people building these widely use.
3. **Publicly usable.** A public repository, package or product page that works today. No dead links, private betas
   or "coming soon".
4. **Licensed, if it is open source.** The repository has a license file or a license in its package manifest.
   Code without a license cannot be reused, so it is left out.
5. **The original.** Not a fork or copy of another project unless it adds real work, and never software that
   cracks, activates or bypasses QuickBooks licensing.

Self-promotion is welcome, as long as the entry meets the criteria and the description is honest.

## Entry format

One line per project, **alphabetical within its group**:

```md
- **[project-name](https://github.com/OWNER/REPO)** ![stars](https://img.shields.io/github/stars/OWNER/REPO?style=flat-square&label=&color=555) — What it does, in one sentence.
```

Rules:

- **Descriptions come from the project itself:** its GitHub description, README or site. Trim and tidy, but do
  not invent features or add numbers the project does not state.
- One sentence, ending with a period. No marketing words such as "the best" or "revolutionary".
- When two projects share a name, add the owner in brackets: `quickbooks-mcp (owner)`.
- Drop the star badge for entries that are not on GitHub.
- Mark an open-source entry ☁️ when it only works with a paid or hosted service.
- No prices: they change too often. Link to the vendor's pricing page instead, if it matters.
- Keep the name as the project publishes it, and match the owner's exact casing in URLs.

## Choosing a section

Sections group by **what a tool is**, then by QuickBooks product:

| Section | Belongs there if… |
|---|---|
| 🎓 Agent Skills & Plugins | it is skills, prompts or a plugin you give an agent |
| 🔌 MCP Servers | it speaks the Model Context Protocol |
| 🧩 AI on the Books | it is an app or agent that does one bookkeeping job with AI (categorizing, bills, collections, reporting) |
| 🖥 CLIs | it is a command-line tool for QuickBooks |
| 📦 Starter Kits & Reference Builds | it is a project you clone or copy to start from |
| 🧱 Building Blocks | it is an SDK or library for building QuickBooks tools |
| ☁️ Hosted & Commercial | it is a paid or hosted service |
| 📚 Reading & Resources | it is an article, guide, specification or comparison |

If an entry fits two sections, put it in the main one and add a `See also` line in the other. A tool that is not
made for QuickBooks but helps in a QuickBooks workflow goes in a 🧭 Adjacent & general-purpose subsection.

## Before you open the pull request

- Check that the link works (`curl -sIL -o /dev/null -w '%{http_code}\n' <url>` should end in `200`).
- Check that the project is not already listed under another name.
- One entry per line keeps the diff readable.
