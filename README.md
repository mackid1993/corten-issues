<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="social-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="social-light.svg">
    <img src="social-light.svg" alt="Corten-Matrix: iMessage on any Matrix client" width="640">
  </picture>
</p>

# Corten-Matrix Issues

This repo is where you report bugs in Corten-Matrix. There's no code here, just the issue tracker.

> **Issues are for bugs in the bridge, not setup help.** Setup questions and "how do I...?" go in the **[community room](https://matrix.to/#/#corten-matrix:beeper.com)**, where people who run the bridge help each other. Issues asking for setup help are closed.

**Downloads, setup instructions and release notes:** https://corten-matrix.com

Official builds come only from that site, signed and checksummed. If you're running a build from anywhere else, please reproduce the problem on an official build before filing.

## One developer. Bugs come first.

Corten-Matrix is built and maintained by **one person**, in their spare time. Bug reports always take priority over feature requests. Serious bugs are worked on as soon as possible; minor ones get fixed when there's time, and that can take a while. Feature requests are read, but they wait, and some won't happen at all.

## Before you file

- **Update first.** Run `corten-matrix update` and check the problem still happens on the latest release.
- **Search the existing issues.** Someone may have hit it already, open or closed.
- **Is it really the bridge?** If the same thing fails in Apple's own Messages app, it's an Apple account problem, not a bridge bug.
- **Setup questions** belong in the [community room](https://matrix.to/#/#corten-matrix:beeper.com). Everything about setting it up is on [corten-matrix.com](https://corten-matrix.com).

## How an issue works

Most bridge bugs can only be fixed by working directly with the person who has them, so we need a private way to reach you. GitHub has no private fields, so it works like this:

1. **Open an issue** with the bug report or feature request form. **Don't put your Matrix ID in it.**
2. **A bot replies** within a few seconds, asking for your Matrix ID.
3. **Within 1 hour, reply with a comment that contains only your Matrix ID**, for example `@you:beeper.com`. Any format is fine (`you:beeper.com`, `you@beeper.com`, a matrix.to link).
4. **The bot deletes that comment within seconds** and passes your ID along privately. It's visible on the page for those few seconds and may show up in email notifications to people watching the repo, so reply with the ID and nothing else.
5. **The bot confirms** it got your ID, and someone will be in touch on Matrix.

### The rules, and why

These apply to everyone, including the developer.

| What happens | Why |
| --- | --- |
| **No Matrix ID within 1 hour:** the issue is closed automatically. | Without a way to reach you, the bug can't be worked on. Open a new issue when you're able to reply. |
| **Matrix ID in the title, the form or any other comment:** the issue is closed and locked, and the ID is removed. | Anything typed into a GitHub issue is public and kept in its edit history. Only the reply comment can be deleted cleanly. |
| **Someone else posts a Matrix ID on your issue:** their comment is removed. | Only the person who opened the issue gives a Matrix ID, and only the way described above. |

### What we may ask for

Many bugs only happen with a particular account, chat history or setup. On Matrix we may ask for your **bridge logs** and your **bridge database**. They contain personal data such as contacts, phone numbers and message text. They're used only to find and fix your bug, never shared, and deleted when the issue is closed. Sending them is your choice, but some bugs can't be fixed without them.

When you paste log lines into an issue, remove phone numbers, email addresses and message text first.

## How issues are prioritized

1. **Serious bugs first:** messages lost or not delivering, the bridge failing to start or log in, anything that breaks it for many people.
2. **Minor bugs next:** cosmetic problems, rare edge cases, things with an easy workaround. These are fixed when there's time. "Any update?" won't speed one up, but new information that helps reproduce it is always welcome.
3. **Feature requests last.** They're read, and good ones get built eventually, but never ahead of a bug.

An issue may be closed if it can't be reproduced, if we can't reach you, or if the problem is outside the bridge.

## Please don't

- Use issues for setup help or general questions. Ask in the [community room](https://matrix.to/#/#corten-matrix:beeper.com).
- Open a new issue for setup help after one was closed as not a bridge bug.
- Post logs, databases or anything private in an issue.
- Open duplicate issues to get attention.

Thanks for helping make Corten-Matrix better.
