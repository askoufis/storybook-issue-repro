# Storybook Issue #{} Reproduction

Heading anchors seem to have broken in Storybook 10.5.0.
Clicking the heading link copy button doesn't seem to scroll to the heading any more.

The `master` branch is pinned to `10.5.0`, while the working `storybook-10.4` branch installs the latest `10.4.x` version (patch-version flexible).

## Reproduction steps

Run `pnpm storybook` and navigate to the `Button/Docs` page.
Clicking a heading anchor copy button should scroll to the anchor, but it doesn't.

Run `git checkout storybook-10.4`, then `pnpm install && pnpn storybook` and navigate to `Button/Docs` again.
Clicking a heading anchor copy button correctly scrolls to the anchor.
