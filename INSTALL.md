# Install ADHD Wise Kit

Takes about 2 minutes. Pick the app you use.

## Claude Desktop, claude.ai or Cowork

You need a Claude Pro plan or higher.

1. Download `adhd-wise-kit-<version>.zip` from your purchase email.
2. In Claude, open **Customize → Plugins → Add → Upload plugin** and choose the zip.
3. In **Settings**, turn on **Code execution and file creation**.
4. Optional but worth it: connect **Gmail**, **Google Calendar** and **Google Drive** in
   Customize → Connectors. The skills work without them, and do much more with them.

To update, upload the new zip from the update email.

## Claude Code

Accept the GitHub invite from your purchase email first, and make sure git can reach
GitHub (`gh auth login`, then `gh auth setup-git`).

```
/plugin marketplace add mostafa-drz/adhd-wise-kit
/plugin install adhd-wise-kit@adhd-wise
```

To get updates automatically, open `/plugin`, go to Marketplaces, select `adhd-wise`,
and turn on auto-update.

## Codex, Cursor, GitHub Copilot, Gemini CLI

Unzip `adhd-wise-kit-<version>-agents-skills.zip` into `~/.agents/skills/`.

## Check it works

Say: "What emails have I been avoiding?" or "Where was I?"

Productivity tools only. Not medical advice or a substitute for professional care.
