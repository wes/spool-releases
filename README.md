# Spool

A fast email client for macOS.

Spool is written in Rust and draws with the GPU, using the same UI framework as
the Zed editor. There is no web view and no Electron anywhere in it. The point
of building it that way is not the stack — it is that a mailbox with a quarter
of a million messages in it feels the same as an empty one.

**[Download the latest release](https://github.com/wes/spool-releases/releases/latest)**

Requires macOS 13 (Ventura) or later. Universal — Apple silicon and Intel.

## Installing

Open the disk image and drag Spool to Applications. The app is signed and
notarized by Apple, so it opens on the first double-click; there is no
right-click-Open ritual and nothing to disable in System Settings.

## What it does

Three panes — mailboxes, messages, the message — driven from the keyboard, with
a command palette for everything that does not have a key. Several accounts at
once, with a unified inbox across them. Full-text search that keeps up with
typing. Conversation threading. HTML mail rendered as styled text rather than
handed to a browser engine. Four themes.

It syncs over IMAP against real servers, and it is quick about it.

## What it does not do yet

**You cannot write mail in it.** Composing, replying and forwarding are not
built; the send engine is, and nothing in the app reaches it. Today Spool is
somewhere to read, search and file mail, and you will need something else open
to answer any of it. That is the next thing being worked on.

Also missing: OAuth for anything but Gmail (elsewhere means an app password),
attachments beyond their names, a contacts screen, and new mail arriving on its
own rather than when you ask.

## Setting up an account

On first launch Spool asks for an account. Gmail signs in with Google. Everyone
else needs the IMAP and SMTP host names and an **app password** — not your
normal one, which most providers will refuse. Passwords are stored in the macOS
keychain.

## Reporting a bug

[Open an issue.](https://github.com/wes/spool-releases/issues/new/choose) The
version from **Spool → About** and what you were doing when it happened are
usually enough to get started.

This repository holds the releases, the changelog and the issue tracker. The
source is not public.
