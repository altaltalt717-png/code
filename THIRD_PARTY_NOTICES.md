# STORM0S third-party notices

Review date: November 27, 2026. **Partial inventory; redistribution clearance is incomplete.**

The root LICENSE covers only eligible original material owned by the STORM0S operator. It does not cover third-party components or override their permissions. Existing notices inside HTML, compressed payloads, and scripts have been preserved.

## Identified bundled libraries

The versions below come from the local build dependencies and were cross-checked against available embedded notices; they do not identify every dependency in every imported app.

| Component | Local version | License | Included notice |
| --- | --- | --- | --- |
| chess.js | 1.4.0 | BSD-2-Clause | licenses/chess.js.txt |
| React | 19.2.4 | MIT | licenses/react.txt |
| React DOM | 19.2.4 | MIT | licenses/react-dom.txt |
| Scheduler | 0.27.0 | MIT | licenses/scheduler.txt |
| use-sync-external-store | 1.7.0 | MIT | licenses/use-sync-external-store.txt |
| Tailwind CSS | 4.3.4 in the 50-game bundle | MIT | licenses/tailwindcss.txt |
| decimal.js-light | 2.5.1 | MIT | licenses/decimal.js-light.txt |
| lucide-react | 1.16.0 | ISC (including upstream notices) | licenses/lucide-react.txt |

chess.js is also embedded directly as `storm-chess-engine`. React-related packages, decimal.js-light, Lucide and chess.js are identified by the `storm-50-games` bundle's license block. Other embedded pages identify Tailwind 4.1.16 and 4.3.3; their exact source correspondence still needs review. Semantic UI 2.5.0 and normalize.css 7.0.0 MIT notices occur in `extra-upload-oct21-11`; their full corresponding notices and provenance remain to be collected.

## GUST and libcurl.js: unresolved source-distribution obligations

`embedded-gust` contains an explicit libcurl.js LGPL v3 notice, copyright 2024 ading2210, and compiled content. That existing component notice is copied to `licenses/gust-libcurl-component-notice.txt`. Official LGPL v3 and GPL v3 texts are provided alongside it.

Source reference recorded in the component: https://github.com/ading2210/libcurl.js
GUST project reference from the supplied app history: https://github.com/nautilus-os/GUST

The libcurl.js notice also identifies libcurl (curl License), mbedTLS (Apache-2.0), cJSON (MIT), zlib (zlib License), Brotli (MIT), and nghttp2 (MIT). Exact versions and the complete corresponding source/build materials were not established in this review. Merely linking an upstream repository or copying license text does not establish that source-distribution, modification, relinking/replacement, or other applicable obligations have been met. The outer GUST application's license also requires verification. Do not treat this bundle as cleared for restrictive redistribution.

## Imported apps, game pages and external services

`THIRD_PARTY_INVENTORY.json` lists compressed payload identifiers, hashes, sizes, and catalog library counts. These are discovery records, not ownership determinations. Some payloads are STORM0S-generated bundles containing third-party libraries; others are imported pages. A copyright keyword match is not a license grant.

Scratch, cinema, YouTube, Spotify, AI, proxy/browser apps, imported games, and runtime-loaded libraries remain under their respective owners' terms and licenses. `embedded-scratch` loads scripts from the 4gamess/scratchrip repository; that fork's underlying Scratch and Machine Learning for Kids code and asset permissions need separate review. `embedded-storm-ai` references rhulha/Gemma3-270m-WebGPU; code, model weights, and hosted services may have different terms.

Some imported port pages contain GPL/AGPL or proprietary notices (including Aleph One/Marathon, Freeciv, OpenMW, and commercial-game references). These findings do not establish which executable code or game data is redistributed. Inspect the actual artifact and dependencies before deciding whether it is a separate aggregate, a combined work, or a link to a remote service.

Catalog entries often fetch third-party HTML and images at runtime. A public GitHub repository, CDN URL, attribution, or lack of a takedown is not permission to redistribute a game or its assets. Hosting a loader does not establish rights to the remote material.

## Images, music and branding

User-supplied photos, memes, character art, sound effects, and music were not verified as original or licensed. In particular, the prepared `music/` folder contains third-party recordings with no permission documentation supplied. Current clicker music uses local MP3 uploads, YouTube embeds, or Dropbox links and does not require that folder; do not upload the prepared recordings without appropriate rights. File names such as "No copyright" are not license evidence.

STORM0S makes no ownership claim here over these materials or third-party trademarks. An app's branding replacement does not change the underlying rights.

## Review limitations and next steps

This is a static notice/provenance review of turtle.html, decoded embedded scripts, the catalog, and available local package licenses. It is not a complete audit of every game, remote script, binary, image, audio recording, or modified upstream source. No unverified component has been silently removed or relicensed.

Before treating the entire distribution as cleared: establish exact upstream versions and licenses, obtain missing permissions, collect required corresponding source and build materials, and replace or omit components whose permissions cannot be established. Preserve third-party notices with every distribution. If copyleft applies to a combined work, comply with it rather than relying on the original-material restriction.
