# Contributing to Awesome Context Engineering

This repo maps AI memory systems, context engineering patterns, and the emerging stack for persistent agent memory.

Contributions should make the landscape easier to compare, not just add more links.

## How To Add a System

1. Pick the most relevant landscape category:
   - `landscape/frontier-platforms.md`
   - `landscape/coding-agents.md`
   - `landscape/local-agent-harnesses.md`
   - `landscape/personal-memory-systems.md`
   - `landscape/memory-infrastructure.md`
   - `landscape/protocols-and-connectors.md`
   - `landscape/team-knowledge-memory.md`
2. Copy `templates/system-profile.md` into `systems/<system-name>.md`.
3. Fill the profile with source-backed research.
4. Add the system to the relevant landscape page.
5. If the system is especially important, add it to the starter table in `README.md`.

## Profile Quality Bar

Every system profile should answer these core questions:

- What does it remember?
- What is the memory scope: session, project, user, team, organization, or cross-agent?
- How is memory written?
- How is memory retrieved?
- How much control does the user have?
- How portable is the memory?
- What are the system's strengths and limitations?
- How does it relate to Membase or the broader universal memory layer pattern?

## Sources

Use primary sources whenever possible:

- Official docs
- Official blog posts
- Product pages
- GitHub repositories
- Technical papers
- Maintainer-written examples

When primary sources are not enough, secondary sources are allowed, but mark them clearly.

## Writing Style

- Be factual and specific.
- Avoid hype and vague claims.
- Prefer comparison-friendly wording.
- Mention uncertainty with `TBD` instead of guessing.
- Keep the `Relationship to Membase` section analytical, not promotional.

## Pull Request Guidelines

- One system profile per PR is preferred.
- Include source links in the profile.
- Explain what category the system belongs to and why.
- Keep unrelated formatting changes out of the PR.

## License Agreement

By contributing, you agree that your contributions will be licensed under the Apache License 2.0, the same license as this project.
