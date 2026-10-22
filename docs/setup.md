# Use in a project

These are manual setup instructions. Creating this repository does not install anything.

1. Inspect the target project's existing AGENTS files and skill organization.
2. Open [the AGENTS template](../templates/AGENTS.md). Merge useful sections into an existing guide, or create a root guide if the project has none. Replace every `[TODO]`, remove inapplicable sections, and verify commands against the project.
3. Choose the skills the project needs: [review-change](../review-change/SKILL.md), [verify-app](../verify-app/SKILL.md), or both. Copy each whole folder into the project's `.agents/skills/` if that is its chosen skill location. Compare any same-named skill before replacing it.
4. Add a short skill index to the project's guide. Fill the verification profile with real commands, journeys, roles, and an evidence location.
5. Keep project facts and private references in that project. Where useful, point the root guide to its own `.agents/references/` files instead of expanding the guide.
6. Review the diff and run the project's relevant checks before relying on the new instructions.

## Skill layout

```text
skill-name/
  SKILL.md          # name and description frontmatter, then workflow
  scripts/          # optional repeatable executable work
  references/       # optional task-specific reading
  assets/           # optional output resources
```

A self-contained skill needs only `SKILL.md`. The discovery description should say what it does and when it applies. Link supporting files from the workflow and copy them with the folder. Keep one maintained source for each fact.

Whether a host discovers project-local skills depends on that host's configuration. Verify discovery there; the presence of a folder alone does not prove installation. Global skill installation, plugin packaging, and synchronization remain separate choices.
