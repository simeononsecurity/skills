# Contributing

Keep this collection focused on repeatable workflows with a clear user trigger and a useful result.

## Propose a skill

Include:

- The audience and request that should activate the skill.
- A concrete outcome or artifact.
- Evidence from a public source or a sanitized, personally owned workflow.
- Why the workflow does not overlap an existing skill.
- Any required tools, host assumptions, and side effects.

## Write the skill

- Use one directory per skill with a `SKILL.md` entrypoint.
- Keep frontmatter `name` aligned with the directory. Describe both the job and when the skill applies.
- Put only decision-changing guidance in `SKILL.md`. Add references or scripts only when the workflow needs them.
- Preserve the user's scope and permissions. Never imply authority to publish, deploy, spend, contact people, delete data, or change live services.
- Use original wording. Do not copy a third-party skill. Link to its canonical source and record license and attribution details when adapting a material idea.
- Exclude secrets, credentials, personal or customer data, employer material, unrelated private projects, private infrastructure identifiers, and private conversation excerpts.

## Validate a change

Run the skill creator validator on each changed skill and check links, names, references, and any helper scripts. Read the final diff and confirm it contains only the intended files. Do not claim a host integration works unless you verified it in that host.

## License

Original contributions use Apache-2.0. A contribution that includes third-party material must keep its own license and notices. Ask before including material whose redistribution terms are unclear.
