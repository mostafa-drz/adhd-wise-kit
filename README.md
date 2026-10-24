# ADHD Wise Kit (private)

Source for the paid ADHD Wise Kit. Buyers get read access to this repo through Polar,
plus a zip download. Do not make this repo public.

- House rules: [SKILLS_GUIDE.md](SKILLS_GUIDE.md)
- Buyer install guide: [INSTALL.md](INSTALL.md)
- `make check` runs the house-rule checks, `make validate` runs Claude Code's validator,
  `make dist` builds the buyer zips into `dist/`.

Bump `version` in `plugins/adhd-wise-kit/.claude-plugin/plugin.json` on every release,
or installed copies won't update.
