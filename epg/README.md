# Electronic Programme Guide (EPG)

This directory contains documentation and references for Electronic Programme Guide (EPG) sources compatible with OpenWave IPTV playlists.

EPG data provides programme information for television channels, allowing compatible IPTV players and media servers to display schedules, programme descriptions, and broadcast times.

---

## Contents

- [About EPG](#about-epg)
- [How It Works](#how-it-works)
- [EPG Sources](#epg-sources)
- [Channel Mapping](#channel-mapping)
- [Supported Formats](#supported-formats)
- [Using EPG Data](#using-epg-data)
- [Contributing EPG Sources](#contributing-epg-sources)
- [Important Notes](#important-notes)

## About EPG

An Electronic Programme Guide provides scheduling information for television channels.

While an M3U playlist tells an IPTV application where to find a channel's stream, an EPG source provides information about what is currently broadcasting and what is scheduled next.

OpenWave IPTV aims to maintain references to compatible EPG sources alongside its channel playlists.

**EPG data and IPTV streams are separate resources.** A working channel stream does not necessarily have an available programme guide.

## How It Works

EPG information is generally associated with channels through unique identifiers.

A typical setup involves three components:

1. **M3U playlist** — Contains channel names, stream URLs, and associated metadata.
2. **EPG source** — Contains programme schedules and channel information.
3. **EPG identifier** — Connects a channel in the playlist to its corresponding entry in the programme guide.

For example:

An IPTV playlist may contain a channel with the identifier `example.tv`.

The corresponding EPG source must contain a channel with the same identifier for the application to associate the programme schedule correctly.

## EPG Sources

EPG sources may be maintained by broadcasters, television listing services, or independent community projects.

When adding an EPG source, document the following information:

| Field | Description |
|---|---|
| Source Name | Name of the EPG provider or project |
| Country | Country or region covered |
| URL | EPG data URL |
| Format | XMLTV or another supported format |
| Coverage | Channels included in the source |
| Last Checked | Date the source was last checked |
| Notes | Relevant limitations or additional information |

Only include sources that can reasonably be used and redistributed as links under their providers' applicable terms.

### Source organisation

EPG references should be organised by country or region where practical.

This makes it easier to identify which sources cover particular channels and avoids unnecessary duplication.

## Channel Mapping

Correct channel mapping is essential for displaying programme information.

The EPG identifier in an M3U playlist should correspond to the channel identifier in the EPG source.

For example:

```text
#EXTINF:-1 tvg-id="example.tv" tvg-name="Example TV",Example TV
https://example.com/stream.m3u8
```

The EPG source must contain a matching channel identifier:

```xml
<channel id="example.tv">
    <display-name>Example TV</display-name>
</channel>
```

If the identifiers do not match, an IPTV application may be unable to associate the programme schedule with the channel.

Channel names alone are not always sufficient for reliable matching.

## Supported Formats

OpenWave IPTV primarily targets the **XMLTV** format for programme guide data.

XMLTV is a widely used format for representing television listings and programme schedules.

Other formats may be documented where they are supported by compatible applications, but compatibility should be verified before inclusion.

## Using EPG Data

EPG sources can be configured in compatible IPTV applications and media servers.

For example, Jellyfin allows users to configure an XMLTV programme guide provider separately from their M3U tuner.

The application then uses the channel identifiers to associate programme information with the available streams.

EPG configuration and playlist configuration may differ between applications. Consult the documentation of your chosen IPTV player or media server for application-specific instructions.

## Contributing EPG Sources

Contributions are welcome.

When submitting a new EPG source, please:

1. Identify the source provider.
2. Provide the EPG URL.
3. Specify the country or region covered.
4. Identify the supported format.
5. Verify that the source is accessible.
6. Confirm that its use as a reference is permitted.
7. Include any known coverage limitations.

Please do not invent channel identifiers or assume that an EPG source covers every channel in a country's playlist.

If a source becomes unavailable or changes its URL, please report it through GitHub Issues.

For further guidance, see [CONTRIBUTING.md](../CONTRIBUTING.md).

## Important Notes

- EPG sources do not provide television streams.
- A channel may be available without having programme guide information.
- Programme schedules may be incomplete, delayed, or inaccurate.
- EPG sources may have geographical or provider-specific restrictions.
- Channel identifiers must match between playlists and EPG data.
- OpenWave IPTV does not host or control third-party EPG services.

All EPG sources remain subject to their respective providers' terms, licences, and restrictions.

---

**OpenWave IPTV - Organised channels, connected schedules.**