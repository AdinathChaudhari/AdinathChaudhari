<h1 align="center">Adinath Chaudhari</h1>

<p align="center">
  <strong>Product and AI</strong><br>
  <em>Engineering at IIT Roorkee, management at INSEAD. I write the spec, then I build the tool.</em>
</p>

I take products from definition and system architecture to shipped software. These repositories are the hands-on side of that: tools I specified, built with AI agents and use myself.

Most began as a problem of my own, however niche. When a project already fits my use case, I improve it upstream. When a good open-source engine exists, I build the workflow around it.

## How I work

- **Spec first.** A written spec comes before any code. AI agents build from it, and I accept each stage against the spec and the tests. [The process, with real traces](https://github.com/AdinathChaudhari/google-drive-suite/blob/main/BUILD-WITH-AI.md).
- **Measured, or marked unmeasured.** Each README states what was measured and names the numbers that do not exist yet.
- **Local and reversible.** Tools run on your own machine, and the ones that change a device ship an undo.

## Latest projects

Three tools for working with AI agents and models, newest first.

<p align="center">
  <a href="https://github.com/AdinathChaudhari/website-mcp"><img src="assets/website-mcp.jpg" width="32%" alt="website-mcp: a browser window with a dotted path that becomes a small glowing tool piece"></a>
  <a href="https://github.com/AdinathChaudhari/preflight-review"><img src="assets/preflight-review.jpg" width="32%" alt="preflight-review: a paper airplane on a runway of code lines beside a checklist"></a>
  <a href="https://github.com/AdinathChaudhari/i-cant-draw"><img src="assets/i-cant-draw.jpg" width="32%" alt="i-cant-draw: a tangled scribble with an arrow leading to a tidy speech bubble of text lines"></a>
</p>

- **[website-mcp](https://github.com/AdinathChaudhari/website-mcp)** turns a website task into a saved, tested tool that runs with no model.<br>
  *Why:* an agent that re-reads the same site pays for a model on every run.<br>
  *Impact:* published on [npm](https://www.npmjs.com/package/website-mcp). The [demo tool](https://github.com/AdinathChaudhari/website-mcp#demo) passes 8 of 8 test cases with no model call.
- **[preflight-review](https://github.com/AdinathChaudhari/preflight-review)** reviews a branch with AI before the push and reports only what it confirmed in the code.<br>
  *Why:* AI reviewers report guesses.<br>
  *Impact:* in the [seeded eval](https://github.com/AdinathChaudhari/preflight-review/blob/main/docs/measurements.md#eval-1--seeded-set-real-models-2026-10-30) on v1.0 it found 7 of 7 planted bugs, with 0 findings on the clean control. Recall on large real diffs is not measured yet.
- **[i-cant-draw](https://github.com/AdinathChaudhari/i-cant-draw)** turns a rough image idea into a ready-to-paste prompt for ChatGPT or Gemini.<br>
  *Why:* a rough idea pasted into an image model comes back with garbled text and a generic picture.<br>
  *Impact:* its README shows [one brief rendered by both engines](https://github.com/AdinathChaudhari/i-cant-draw#see-it-work) with the title text intact. The illustrations on this page were made with it.

## Passion projects

Built for my own use first.

<p align="center">
  <a href="https://github.com/AdinathChaudhari/audiobook-maker-pro"><img src="assets/audiobook-maker-pro.jpg" width="32%" alt="audiobook-maker-pro: a small character in headphones sitting beside a book marked with a sound wave"></a>
  <a href="https://github.com/AdinathChaudhari/google-drive-suite"><img src="assets/google-drive-suite.jpg" width="32%" alt="google-drive-suite: Drivedeck, four self-hosted tools for Google Drive"></a>
  <a href="https://github.com/AdinathChaudhari/markdown-studio"><img src="assets/markdown-studio.jpg" width="32%" alt="markdown-studio: a single sheet rising out of its app tile, plain marks becoming set type"></a>
</p>

- **[audiobook-maker-pro](https://github.com/AdinathChaudhari/audiobook-maker-pro)** turns a folder of audio, a YouTube video or a playlist into one chapterized audiobook, tuned for an iPod.<br>
  *Why:* I listen to long recordings on an iPod. Generic converters miss the details an old player depends on, and each of those details cost me a broken book.<br>
  *Impact:* books over 20 hours are [split at chapter boundaries](https://github.com/AdinathChaudhari/audiobook-maker-pro#faq) with no re-encode, because older iPods stop resuming very long books.
- **[google-drive-suite](https://github.com/AdinathChaudhari/google-drive-suite)** is four self-hosted tools for Google Shared Drives: bulk download, parallel upload, streaming to a Fire TV app and automatic offload.<br>
  *Why:* large Shared Drive libraries are slow to move and awkward to watch through the browser.
- **[markdown-studio](https://github.com/AdinathChaudhari/markdown-studio)** reads, edits and typesets Markdown offline, with tables and LaTeX, as a 1 MB Mac app or a single HTML file.<br>
  *Why:* opening a browser just to read a Markdown file costs more memory than the file deserves.<br>
  *Impact:* the [Mac app](https://github.com/AdinathChaudhari/markdown-studio/releases/latest) measured about 100–126 MB with a document open, and 289 tests run with no network.

Also built for myself:

- **[ipod-movie-maker](https://github.com/AdinathChaudhari/ipod-movie-maker)** prepares video for an iPod touch and checks each file against the device's decoder limits.
- **[housewatch](https://github.com/AdinathChaudhari/housewatch)** counts whole-house data usage from a router. A stretch it cannot prove is recorded as `unknown`, never estimated.
- **[orchard-tv](https://github.com/AdinathChaudhari/orchard-tv)** is an Apple TV-style home screen for a Fire TV Stick, with a reset back to the stock launcher.

## Open source

**Improving what I use.** When a project fits my use case, I read it properly and then propose an improvement.

- **[i-have-adhd](https://github.com/ayghri/i-have-adhd)**, a skill that makes a coding agent lead with the answer. I proposed two rules drawn from W3C cognitive accessibility guidance ([pull request](https://github.com/ayghri/i-have-adhd/pull/21)). It later inspired i-cant-draw.
- **[antivibe](https://github.com/mohi-devhub/antivibe)**, a skill that explains code so the reader learns it. I proposed a map mode for large codebases ([pull request](https://github.com/mohi-devhub/antivibe/pull/11)).
- **[torlink](https://github.com/baairon/torlink)**, a terminal torrent client. I proposed an opt-in setting that routes its searches through Tor ([pull request](https://github.com/baairon/torlink/pull/107)).

**Building on good engines.** I do not rewrite a good engine. I build the workflow around it.

- **[anydl](https://github.com/AdinathChaudhari/anydl)** on yt-dlp, streamlink and aria2c. One prompt takes any link and routes it to the right engine.
- **[streamlist](https://github.com/AdinathChaudhari/streamlist)** on yt-dlp and FFmpeg. Playlists become tagged M4A files, and re-runs fetch only what is missing.
- **[apple-to-ytmusic](https://github.com/AdinathChaudhari/apple-to-ytmusic)** on ytmusicapi. It mirrors Apple Music playlists to YouTube Music and never deletes anything.
- **[video-loop-extractor](https://github.com/AdinathChaudhari/video-loop-extractor)** on yt-dlp and FFmpeg. It finds a video's repeating loop and extracts one seamless clip.
- **[file-translator](https://github.com/AdinathChaudhari/file-translator)** on deep-translator. It renames a folder across languages from one edited sample, with an undo.

---

<p align="center"><a href="https://github.com/AdinathChaudhari?tab=repositories">All repositories</a>. Most READMEs include a transcript of a real run.</p>
