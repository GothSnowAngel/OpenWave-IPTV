# OpenWave IPTV

**An open, community-maintained collection of IPTV playlists and channel information.**

OpenWave IPTV aims to make publicly available IPTV streams easier to discover, organise, and use. The project brings together channel information from different countries and categories into structured playlists that can be used with compatible IPTV players and media servers.

Our goal is to create a resource that is accessible, transparent, and maintained through community contributions.

---

## Contents

- [About](#about)
- [Features](#features)
- [Using the Playlists](#using-the-playlists)
- [Channel Information](#channel-information)
- [Contributing](#contributing)
- [Stream Availability](#stream-availability)
- [Legal Notice](#legal-notice)
- [Licensing](#licensing)
- [Disclaimer](#disclaimer)

---

## About

OpenWave IPTV is a community-driven IPTV playlist project.

Rather than hosting or broadcasting television channels ourselves, we organise and maintain references to streams made available by their respective providers.

The project is intended for:

- IPTV users looking for organised channel playlists.
- Home media server enthusiasts.
- IPTV collectors and hobbyists.
- Developers building IPTV-related tools.
- Contributors interested in maintaining channel information.

Whether you're using Jellyfin, Kodi, VLC, or another compatible application, OpenWave IPTV aims to make finding and organising channels a little easier.

## Features

- **Country-based playlists** — Find channels organised by country.
- **Category-based playlists** — Browse channels by content category.
- **Combined playlist** — Access all included channels from one playlist.
- **Channel metadata** — Maintain information such as channel names, languages, categories, and EPG identifiers.
- **Community contributions** — Help add, update, and verify channel information.
- **Availability checks** — Support the identification of unavailable or outdated streams.

## Using the Playlists

OpenWave IPTV playlists use the M3U format and are intended for compatible IPTV applications.

You can use an individual country or category playlist, or use the combined `all.m3u` playlist.

### Available playlists

| Playlist | Description |
|---|---|
| `all.m3u` | All included channels |
| `countries/netherlands.m3u` | Channels from the Netherlands |
| `countries/belgium.m3u` | Channels from Belgium |
| `countries/germany.m3u` | Channels from Germany |
| `countries/united-kingdom.m3u` | Channels from the United Kingdom |
| `countries/france.m3u` | Channels from France |
| `countries/spain.m3u` | Channels from Spain |
| `countries/japan.m3u` | Channels from Japan |
| `countries/south-korea.m3u` | Channels from South Korea |

Additional playlists may be introduced as the collection grows.

### Direct playlist URLs

Once published, playlists can be accessed through GitHub's raw file URLs.

For example:

```text
https://raw.githubusercontent.com/GothSnowAngel/OpenWave-IPTV/main/playlists/all.m3u
```

## Channel Information

Channel information is maintained centrally to help keep playlists consistent.

Where available, entries may include:

| Field | Description |
|---|---|
| Channel ID | Unique identifier within the project |
| Channel Name | Official or commonly recognised channel name |
| Country | Country of origin |
| Language | Primary broadcast language |
| Category | Channel classification |
| Stream URL | Address of the publicly available stream |
| Logo | Channel logo reference, where permitted |
| EPG ID | Electronic Programme Guide identifier |
| Status | Current verification status |
| Source | Original source of the stream information |

Channel statuses help contributors and users understand the reliability of an entry.

- **Verified** — Stream has been checked and confirmed to work.
- **Unverified** — Stream has been added but has not yet been confirmed.
- **Unavailable** — Stream was checked and could not be accessed.

A successful availability check does not guarantee uninterrupted playback.

## Contributing

OpenWave IPTV welcomes contributions from the community.

You can help by:

- Submitting new publicly accessible channel streams.
- Updating outdated stream URLs.
- Reporting unavailable channels.
- Correcting channel names and metadata.
- Adding permitted channel logos.
- Improving scripts and documentation.
- Helping verify existing entries.

Before submitting a contribution, please ensure that:

1. The stream is publicly accessible.
4. You provide the original source wherever possible.
5. You do not submit personal information, private streams, or credentials.

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

## Stream Availability

IPTV streams can change, become unavailable, or be removed by their providers.

OpenWave IPTV does not guarantee:

- That every stream will work.
- That streams will remain available.
- That streams will be available in every geographical region.
- That streams will work with every IPTV application.
- That programme information or EPG data will always be accurate.

Contributors are encouraged to report broken links and help keep the collection current.

## Legal Notice

OpenWave IPTV does not host, broadcast, retransmit, or control the television streams referenced in its playlists.

The project provides organisational information and links to streams made available by third parties.

The presence of a stream in this repository does not imply ownership, endorsement, or affiliation with its broadcaster or provider.

All contributors are responsible for ensuring that their submissions comply with applicable laws and the relevant providers' terms and permissions.

Channel names, logos, trademarks, broadcast content, and other third-party materials remain the property of their respective owners.

## Licensing

OpenWave IPTV uses different licensing arrangements for original project materials:

- **Source code:** MIT License.
- **Original channel metadata and playlist compilations:** CC0 1.0 Universal, where applicable.
- **Third-party logos and other external materials:** Remain subject to their respective owners' copyright and licensing terms.

These licences do not grant permission to redistribute television broadcasts or other third-party content.

See the repository's licence files and notices for further details.

## Disclaimer

OpenWave IPTV is an independent, community-maintained project.

It is not affiliated with, endorsed by, or sponsored by any television broadcaster, IPTV provider, or streaming service referenced in the repository.

The project is provided on an *as-is* basis, without guarantees of availability, accuracy, or suitability for any particular purpose.

**Use the resources responsibly and respect the rights of content providers.**

---

*OpenWave IPTV - Open access to organised IPTV resources.*
