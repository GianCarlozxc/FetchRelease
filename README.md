# Fetch downloads

Fetch is a Windows download manager with live progress and speed, automatic browser handoff, pause/resume, download history, animations, and optional sounds.

**[Download Fetch Setup](https://github.com/GianCarlozxc/FetchRelease/releases/latest/download/Fetch-Setup-1.0.19.exe)**

**[Download the portable ZIP](https://github.com/GianCarlozxc/FetchRelease/releases/latest/download/Fetch-1.0.19-with-extensions.zip)**

The installer creates a desktop shortcut and configures the Windows browser connector. Both downloads include the Chromium and Firefox browser extensions. Enable the included extension once in each browser; Fetch can then open automatically when a supported download starts, including when Fetch was closed.

Open Fetch's Settings and choose the globe icon for browser setup. Chrome, Edge, and Brave use Developer mode → Load unpacked. Firefox's development extension is loaded as a temporary add-on and must be loaded again after a browser restart.

**Update inside Fetch:** Open Settings ? Check for updates, download a newer version, then choose Install and restart. Fetch verifies the installer and retains your history, settings, and saved files. Version 1.0.0 users must install 1.0.1 once to get this feature.

**Version 1.0.2:** Prevents duplicate browser downloads by pausing the browser transfer before Fetch takes over. Reload Fetch in `brave://extensions` (or your browser's extensions page) after updating.

**Version 1.0.3:** Speeds up updates by reusing unchanged runtime files, shows installation progress, and reopens Fetch visibly after installing.

**Version 1.0.4:** Verifies installed files and the version/build that actually restarts. All version labels use the running app version. Portable updates from 1.0.4 onward replace the current portable copy in its existing folder. Older portable updaters migrate to the installed app; use the desktop shortcut afterward.

**Version 1.0.5:** Fixes the Windows update helper stopping before installation. Fetch waits for helper startup and verifies installed files and the restarted version/build. If an older updater closes without updating, install 1.0.5 once using the setup download.

**Version 1.0.6:** Removes the extra version label from the footer?s right side. The installed version is available in Settings and the sidebar.

**Version 1.0.7:** In-app updates install silently without a separate Fetch Setup window, then automatically reopen the verified new version. The setup wizard remains available for normal first-time installation.

**Version 1.0.9:** Adds file-type icons and image previews, plus right-click commands to download images, media, and links directly with Fetch. Reload the Fetch extension after updating to enable the new commands.

**Version 1.0.10:** Chrome, Edge, and Brave wait for Fetch to accept and cancel the browser download before continuing to the save dialog. Reload the Fetch browser extension after updating. If a handoff fails, normal browser saving remains available. Firefox retains its existing handoff because it does not expose that early filename hook.

**Version 1.0.11:** Replaces dashboard headings with 2D icons, shows received storage and progress for unfinished downloads, adds a live 60-second transfer-speed graph, and displays completed file and byte totals.

**Version 1.0.12:** Handles invalid redirects safely, resets speed during download stalls, adds known extensions to extensionless downloads, and corrects fractional byte-speed formatting. Existing names and resumed download bytes are preserved.

**Version 1.0.13:** Shows connected browsers and extension-version notices, adds copyable setup-folder paths, and retries temporary download failures up to three times with a countdown. Pause, cancel, removal, and app closure stop queued retries. Reload the Fetch extension after updating to activate version 1.4.0 reporting. Store submission materials are prepared; browser-store publishing/signing and store-managed updates are not live yet.

[Browser integration privacy policy](privacy.md).

**Version 1.0.14:** Adds a remembered browser picker for Chrome, Brave, Firefox, and Edge in Settings browser setup, with matching instructions, connection status, extension-folder actions, and copyable settings addresses.

**Version 1.0.15:** The extension button shows Connected when Fetch is connected and Connect to Fetch otherwise. The popup refreshes every three seconds and checks status without launching a closed app; clicking Connect still opens or reconnects Fetch. Reload the extension after updating to activate version 1.4.1.

**Version 1.0.16:** Adds real .torrent and BitTorrent v1 magnet downloads, with actual filenames, progress, speed, peers and seeders. A shared queue limits simultaneous transfers to 1–10 (default 3), supports waiting-download priorities, and adds Pause all / Resume all. Torrent contents and resume files are preserved on pause or removal. The separate aria2 engine and its licenses/source reference are included.

Choose Add torrent or Magnet link in Fetch. Browser extension 1.5.0 can send magnet links through the right-click Download link with Fetch command; captured .torrent downloads automatically start their contents. Reload the included extension after updating. Normal magnet clicks follow your Windows default app. Torrents need reachable peers or web seeds, can upload pieces while downloading, and stop seeding on completion.

**Version 1.0.17:** Webpage magnet-link clicks go directly to Fetch through extension 1.5.1. Fetch opens if closed; the extension prevents the default torrent handler from launching alongside it, avoids duplicate pending handoffs, and shows errors on the webpage. Left and middle clicks, nested elements and embedded frames are supported. Disabled capture, private windows and ordinary links keep their normal behavior.

After updating, reload the Fetch extension and refresh already-open webpages. This captures actual magnet URLs in links or data-magnet/data-url/data-href attributes. Buttons that construct links only inside webpage JavaScript may require copying the magnet into Fetch. All 100 automated tests and real Brave click/handoff checks passed.

**Version 1.0.18:** Adds Windows MAGNET registration so Fetch receives links even when a webpage constructs them inside JavaScript. Cold launches queue the incoming link until Fetch is ready; an open instance receives it directly. Duplicate pending handoffs and active torrent entries are avoided. Settings now includes Use Fetch for magnet links and default-handler status.

After updating, reload extension 1.5.2 and refresh open webpages. If Windows still opens µTorrent or another saved default, choose Fetch for MAGNET through Settings → Use Fetch for magnet links. Windows' protected default-app choice is preserved. This release also fixes Unchecked runtime.lastError: Invalid downloadId while keeping successful browser transfers free of Save As prompts and duplicate downloads. All 105 automated tests, hidden UI checks and real Brave tests passed.

**Version 1.0.19:** Keeps magnet Sending status visible until handoff finishes, adds native-connector and extension-reply timeouts, and shows persistent errors with recovery steps. Handles synchronous Extension context invalidated errors from stale webpages and missing background replies without leaving Sending stuck. Fetch comes forward before torrent-engine startup.

Includes extension 1.5.3. After updating, reload the Fetch extension and refresh open webpages. Check Fetch's download list before retrying a timed-out link. All 109 automated tests and real Brave handoff checks passed, including a local test magnet sent from the reported HTTPS page to the real torrent engine. The original user-specific stalled handoff was not reproduced; this release improves error handling and visibility.

Release downloads include **SHA256SUMS.txt** for integrity verification. [See all releases](https://github.com/GianCarlozxc/FetchRelease/releases).

