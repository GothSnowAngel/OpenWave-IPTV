# Contributing to OpenWave IPTV

Thank you for your interest in contributing to OpenWave IPTV!

OpenWave IPTV is a community-maintained project, and its usefulness depends on accurate information, responsible submissions, and active maintenance.

Whether you're adding a new channel, correcting existing information, reporting a broken stream, or improving the project's tools, your contributions are welcome.

Please read the guidelines below before submitting changes.

---

## Contents

- [Ways to Contribute](#ways-to-contribute)
- [Before Submitting](#before-submitting)
- [Adding a Channel](#adding-a-channel)
- [Updating an Existing Channel](#updating-an-existing-channel)
- [Reporting Broken Streams](#reporting-broken-streams)
- [Channel Metadata Standards](#channel-metadata-standards)
- [Stream and Source Requirements](#stream-and-source-requirements)
- [Pull Request Guidelines](#pull-request-guidelines)
- [What We Do Not Accept](#what-we-do-not-accept)
- [Questions and Discussions](#questions-and-discussions)

---

## Ways to Contribute

There are several ways to help maintain OpenWave IPTV.

### Add new channels
Submit publicly accessible streams that are appropriate for inclusion in the project.

### Update channel information
Correct channel names, countries, languages, categories, EPG identifiers, and other metadata.

### Report unavailable streams
Let us know when an existing stream no longer works or has changed.

### Improve documentation
Help make the project easier to understand and use.

### Improve project tools
Contribute to playlist generation, validation scripts, and other supporting utilities.

---

## Before Submitting

Please check the existing repository before submitting a new channel.

In particular:

- Make sure the channel isn't already listed.
- Check whether the stream URL is already present.
- Verify that the channel information is accurate.
- Include the original source of the stream.
- Ensure that the submission complies with the requirements in this document.

Duplicate entries and incomplete submissions may be rejected or returned for correction.

---

## Adding a Channel

When submitting a new channel, provide as much of the following information as possible:

| Field | Required | Description |
|---|---|---|
| Channel Name | Yes | Official or commonly recognised name |
| Country | Yes | Country of origin |
| Language | Yes | Primary broadcast language |
| Category | Yes | News, Sports, Entertainment, Music, Regional, etc. |
| Stream URL | Yes | Direct URL to the stream |
| Logo | No | Logo URL, where permitted |
| EPG ID | No | Corresponding programme guide identifier |
| Source | Yes | Original source of the stream |

Please use the project's existing metadata conventions.

If you cannot verify a particular field, leave it unspecified rather than guessing.

### Stream verification

Before submitting a stream:

1. Open the stream using a compatible IPTV player.
2. Confirm that the channel plays.
3. Check that the stream corresponds to the submitted channel.
4. Record the source from which the stream was obtained.
5. Note any relevant geographical or access restrictions.

A stream that responds to an HTTP request is not necessarily a playable television stream.

---

## Updating an Existing Channel

If a channel's information changes, please update the existing entry rather than creating a duplicate.

Examples include:

- A new stream URL.
- A changed channel name.
- A corrected EPG identifier.
- A different broadcast language.
- A changed channel category.
- An updated logo reference.

When replacing a stream URL, include the reason for the change and, where possible, evidence that the replacement works.

---

## Reporting Broken Streams

If you encounter an unavailable stream, please report it through the repository's GitHub Issues.

Include:

- Channel name.
- Country.
- Playlist in which it appears.
- Stream URL or channel identifier.
- Date and time you checked it.
- Any error message or relevant information.

Please distinguish between a permanently unavailable stream and a temporary playback issue.

Streams may be inaccessible because of maintenance, geographical restrictions, provider changes, or temporary outages.

---

## Channel Metadata Standards

Consistency is important for keeping playlists organised.

Please follow these conventions:

- Use official channel names where possible.
- Use ISO 3166-1 alpha-2 country codes where applicable.
- Use recognised language identifiers.
- Keep category names consistent with existing project categories.
- Avoid unnecessary abbreviations.
- Do not invent EPG identifiers.
- Use stable identifiers wherever possible.
- Include source information for every submission.

If a channel broadcasts in multiple languages or has regional variants, make those distinctions clear.

---

## Stream and Source Requirements

OpenWave IPTV aims to reference streams that are legitimately made available by their providers.

Contributors must ensure that submitted streams:

- Are publicly accessible without bypassing authentication.
- Are not obtained through unauthorised access.
- Are not taken from private or personal IPTV subscriptions.
- Do not require circumventing paywalls or access controls.
- Are submitted with their original source information.
- Can reasonably be included as links under the provider's applicable terms and permissions.

**Public accessibility does not automatically mean redistribution is authorised.**

If you are unsure whether a stream can be included, do not submit it until its permissions have been established.

---

## Pull Request Guidelines

All changes should be submitted through GitHub Pull Requests.

When opening a pull request:

1. Provide a descriptive title.
2. Explain what you changed.
3. Identify the affected channels or playlists.
4. Include sources for newly submitted streams.
5. Mention any verification performed.
6. Confirm that your changes follow these guidelines.

Please keep pull requests focused. Separate unrelated changes into different submissions where practical.

### Suggested pull request titles

- `Add: Netherlands – Example Channel`
- `Update: Belgium – Example Channel stream`
- `Fix: Incorrect EPG identifier`
- `Remove: Unavailable stream`
- `Docs: Improve installation instructions`
- `Scripts: Improve playlist validation`

Maintainers may request additional information, suggest corrections, or decline submissions that do not meet the project's requirements.

---

## What We Do Not Accept

The following submissions are not permitted:

- Private or credential-protected streams.
- Malware, malicious links, or suspicious scripts.
- Misleading or deliberately incorrect channel information.
- Duplicate entries submitted without justification.
- Content that violates applicable laws or third-party rights.

Maintainers reserve the right to remove entries or reject contributions that do not comply with these guidelines.

---

## Questions and Discussions

If you have questions about contributing, encounter an issue, or want to suggest an improvement, please use the repository's GitHub Issues or Discussions, where available.

For bug reports, please provide enough information for maintainers to reproduce the problem.

For feature suggestions, explain what you would like to see and how it would benefit the project.

---

**Thank you for helping make OpenWave IPTV a useful, organised, and responsibly maintained community resource.**
