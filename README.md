# kf-stack

A small personal toolkit for carrying agent instructions, skills, and working preferences between projects.

This foundation distills existing local conventions. It contains a project instruction template and two portable review/verification skills. It is a file-based toolkit; plugin packaging remains a pending choice.

## Start here

1. Read [preferences](docs/preferences.md) and [pending choices](docs/pending.md).
2. Adapt [templates/AGENTS.md](templates/AGENTS.md) to one project using the [setup guide](docs/setup.md).
3. Select [review-change](review-change/SKILL.md) for change reviews or [verify-app](verify-app/SKILL.md) for application verification.

Each skill is a folder containing `SKILL.md`. Keep supporting resources with their skill. Project-local copies can live in `.agents/skills/`; task-specific knowledge can live in `.agents/references/`.

The optional [Things AppleScript adapter](https://github.com/keyanfayaz/things-applescript) is maintained separately. It is not installed by this toolkit.

No installer, background service, credentials, project data, or global configuration is included. Source paths and detailed provenance are retained outside this repository. No third-party framework code is vendored.
