<p align="center">
  <img src="logo.png" width="96" alt="VideoCatch owl mascot">
</p>

<h1 align="center">VideoCatch</h1>

<p align="center">
  Free social media video and photo downloader.<br>
  Paste a link, get the original file, straight from the platform's own servers.<br>
  <a href="https://videocatch.org">videocatch.org</a>
</p>

## Disclosure and purpose

This repository is maintained by the team behind VideoCatch. It is the project's official
public directory, not an independent review or third-party ranking. Its purpose is to give
readers and crawlers one accurate, human-readable map of the live tool pages on the site.
A public GitHub listing here does not guarantee search-engine indexing, ranking, or
backlink value — those outcomes are outside the maintainer's control.

This directory is kept in sync with the site's live sitemap. When a platform page is added,
removed, or renamed, this README is updated to match rather than left pointing at a stale
route.

## What it does

VideoCatch reads a public post the way a signed-out visitor would and hands back every file it holds: the best MP4 encodes, the full-resolution photos of a carousel, or both when a post mixes them. Multi-item posts get a "Download all as zip" button that packs the files in your browser.

There is no account. Video downloads are streamed through the VideoCatch Worker from the platform CDN without saving or transcoding the video. Images may download directly from the CDN. Public post metadata and media URLs are cached in Cloudflare D1 and reused for one hour; expired entries are no longer read, but are not automatically deleted.

## Supported platforms

| Platform | Page |
|---|---|
| X / Twitter (videos and GIFs) | [Twitter video downloader](https://videocatch.org/twitter-video-downloader) · [GIF](https://videocatch.org/twitter-gif-downloader) |
| Instagram (videos, reels, photos) | [Instagram video downloader](https://videocatch.org/instagram-video-downloader) · [Reels](https://videocatch.org/instagram-reels-downloader) |
| Threads | [Threads video downloader](https://videocatch.org/threads-video-downloader) |
| RedNote / 小红书 | [RedNote video downloader](https://videocatch.org/rednote-video-downloader) |
| Pinterest (videos, pins, idea pins) | [Pinterest video downloader](https://videocatch.org/pinterest-video-downloader) · [Images](https://videocatch.org/pinterest-image-downloader) |
| Snapchat Spotlight | [Snapchat video downloader](https://videocatch.org/snapchat-video-downloader) |
| Facebook (videos and reels) | [Facebook video downloader](https://videocatch.org/facebook-video-downloader) · [Reels](https://videocatch.org/facebook-reels-downloader) |
| TikTok (videos and photo posts) | [TikTok video downloader](https://videocatch.org/tiktok-video-downloader) |
| Twitch clips | [Twitch clip downloader](https://videocatch.org/twitch-clip-downloader) |

YouTube is left out on purpose. Private posts, stories that need a login, and content the creator has restricted are not reachable.

## Principles

- **Original files, not re-encodes.** You get the encode the platform serves its own player, at every quality it offers.
- **No stored videos.** The Worker forwards video bytes without saving a copy. Metadata cache reuse lasts one hour; expiry does not delete the stored row.
- **No account; analytics disclosed.** The site loads Cloudflare Web Analytics, Google Analytics (GA4), Microsoft Clarity (including session replays and heatmaps) and Ahrefs Analytics. See the [privacy policy](https://videocatch.org/privacy).
- **Rights holders are heard.** Takedown requests go to hello@videocatch.org and are answered; see the [copyright and takedown policy](https://videocatch.org/dmca).

## Links

- Website: https://videocatch.org
- Contact: hello@videocatch.org
- About: https://videocatch.org/about
- Terms: https://videocatch.org/terms
- DMCA / takedown policy: https://videocatch.org/dmca

This repository is the public home of the VideoCatch project: the README, the logo, and release notes. The application source is not published here.

## License

This repository's documentation text (this README) is available under [CC BY 4.0](LICENSE). This does not extend to videocatch.org's site content, application source, or trademarks.
