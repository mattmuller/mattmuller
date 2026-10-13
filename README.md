# Matt Muller

Technology Leader, solutions architect and AI engineer. I've spent most of my career in consultancies and agencies, turning a client's problem into something that works, and these days I do much of that with AI agents.

I'm most interested in the layer that makes AI-built software safe to rely on: orchestrating agents, and proving their work instead of trusting it.

I've recently started contributing more to open source, mostly security and reliability fixes for the AI and database tools I use every day.

## Projects

- **[RLS Saboteur](https://github.com/mattmuller/rls-saboteur)**: mutation testing for Postgres row-level security. It breaks each policy on purpose, one at a time, and reports which breaks your tests did not notice. Works with Supabase and plain Postgres, with a CLI, a GitHub Action and a Claude Code plugin.

## Contributions

- [NVIDIA SkillSpector #91](https://github.com/NVIDIA/SkillSpector/pull/91) (merged): SkillSpector, NVIDIA's security scanner for AI agent skills, crashed when a model returned its findings as a JSON string instead of an array. The fix repairs the response so the report is still written. Found on real scans through a multi-provider gateway.

New security lints for [Supabase Splinter](https://github.com/supabase/splinter), the linter behind Supabase's Security Advisor:

- [#198](https://github.com/supabase/splinter/pull/198): a policy calls a function the querying role cannot execute
- [#199](https://github.com/supabase/splinter/pull/199): a custom role inherits `anon` or `authenticated`
- [#200](https://github.com/supabase/splinter/pull/200): a column-level revoke that a table-level grant overrides
- [#201](https://github.com/supabase/splinter/pull/201): `current_user` inside a security definer function
