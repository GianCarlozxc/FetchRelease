# Fetch downloads

Fetch is a Windows download manager with live progress and speed, automatic browser handoff, pause/resume, download history, animations, and optional sounds.

**[Download Fetch Setup](https://github.com/GianCarlozxc/FetchRelease/releases/latest/download/Fetch-Setup-1.0.5.exe)**

**[Download the portable ZIP](https://github.com/GianCarlozxc/FetchRelease/releases/latest/download/Fetch-1.0.5-with-extensions.zip)**

The installer creates a desktop shortcut and configures the Windows browser connector. Both downloads include the Chromium and Firefox browser extensions. Enable the included extension once in each browser; Fetch can then open automatically when a supported download starts, including when Fetch was closed.

Open Fetch's Settings and choose the globe icon for browser setup. Chrome, Edge, and Brave use Developer mode → Load unpacked. Firefox's development extension is loaded as a temporary add-on and must be loaded again after a browser restart.

**Update inside Fetch:** Open Settings ? Check for updates, download a newer version, then choose Install and restart. Fetch verifies the installer and retains your history, settings, and saved files. Version 1.0.0 users must install 1.0.1 once to get this feature.

**Version 1.0.2:** Prevents duplicate browser downloads by pausing the browser transfer before Fetch takes over. Reload Fetch in `brave://extensions` (or your browser's extensions page) after updating.

**Version 1.0.3:** Speeds up updates by reusing unchanged runtime files, shows installation progress, and reopens Fetch visibly after installing.

**Version 1.0.4:** Verifies installed files and the version/build that actually restarts. All version labels use the running app version. Portable updates from 1.0.4 onward replace the current portable copy in its existing folder. Older portable updaters migrate to the installed app; use the desktop shortcut afterward.

**Version 1.0.5:** Fixes the Windows update helper stopping before installation. Fetch waits for helper startup and verifies installed files and the restarted version/build. If an older updater closes without updating, install 1.0.5 once using the setup download.

Release downloads include **SHA256SUMS.txt** for integrity verification. [See all releases](https://github.com/GianCarlozxc/FetchRelease/releases).

