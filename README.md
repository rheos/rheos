# Robin Goodwin

I'm a senior full-stack developer based in British Columbia, Canada, and the founder of [Novadiem Studio](https://novadiem.com). I build production web applications and tools for agent-assisted work.

I've worked in software for more than 25 years and was the first developer on MyFonts.com. I design systems, write code and keep them running. My recent agent projects use durable records, isolated workspaces or review contexts, and explicit access boundaries.

## Selected work

### rheoStream

Self-hosted agent workflows with one Postgres database per workspace, leased background jobs and a transactional outbox. Web and MCP clients share the same service boundary. Recallatron stores memory that can be corrected and superseded, with hybrid retrieval using local embeddings. Redaction controls what reaches a model; private workspace data stays outside the public repository.

The core and Recallatron are implemented. Leads, Current and Relationships remain stubs. Job enqueue crosses two databases without a shared transaction; a missed scheduling mark can delay work until reconciliation.

[Code and status](https://github.com/rheos/rheostream) · [Architecture tour](https://github.com/rheos/rheostream/blob/main/docs/architecture/code-tour.md)

### The Bureau

Multi-agent engineering with cold review in isolated contexts. Reviewers receive evidence packets without the conversation that produced the work. Artifact hashes bind responses to the reviewed files; coverage checks flag missing documents and claims to have read unstaged files. Run state, decisions and handoffs persist on disk so work can resume after an interruption.

This is the internal system I use across studio projects, published for inspection. It is not a supported self-serve product and has no open-source license. The checks validate reported review coverage, not whether a model understood the evidence or reached a sound verdict.

[Code and workflow](https://github.com/Novadiem-Studio/bureau) · [Review tour](https://github.com/Novadiem-Studio/bureau/blob/main/docs/checkpoint-review-tour.md) · [Case study](https://novadiem.com/work-bureau)

### Nutrifax

Production software that turns recipes into Canadian nutrition labels using government nutrient data. I designed and built the application, including the calculation pipeline, PDF generation and subscription billing.

[Product](https://nutrifax.app) · [Case study](https://novadiem.com/work-nutrifax)

### GrowOperative and FOAF

A local-food exchange using trusted relationships and mutual credit. I designed the original system and led the early development team. Later, I took over the development work and rebuilt the platform. The FOAF Ruby service implements the credit ledger; the broader protocol remains in development.

[Product](https://growoperative.app) · [Protocol code](https://github.com/FOAF-Foundation/foaf-protocol-ruby) · [Case study](https://novadiem.com/work-growoperative)

## Smaller tools

- [M.O.T.](https://github.com/rheos/mot) turns messages and agent activity into durable tickets with searchable history. I use it as my operations desk.
- [gsc-mcp](https://github.com/rheos/gsc-mcp) gives agents read-only access to Google Search Console analytics and URL inspection.

## Working stack

Python, TypeScript, Ruby, Next.js, React Native, FastAPI, Rails, MySQL, PostgreSQL, SQLite, Docker, AWS and Linux.

## Work with me

[More work and case studies](https://novadiem.com/work) · [Contact](https://novadiem.com/contact)
