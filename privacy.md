# Fetch Browser Integration privacy policy

Fetch Browser Integration sends supported file downloads to the Fetch Windows application on the same computer. It has no analytics, advertising, or telemetry service.

The extension reads the download URL, suggested filename, referring page, and cookies for the specific download URL when needed to download an authenticated file. These are sent only to the paired Fetch application at 127.0.0.1 over localhost. For unfinished downloads, Fetch can retain these request headers encrypted with Windows DPAPI so authenticated transfers can resume after reopening the app. They are not stored as plaintext or exposed to the interface; completed or removed entries discard their encrypted headers. If encryption is unavailable, headers stay only in memory. Fetch stores download URLs and progress in local history. Cross-origin redirects remove cookies and referrer headers. Sending the same paused or failed file again from the browser refreshes that entry's session without adding a duplicate.

The extension stores its local pairing token, enable/disable preference, connection details, and last transfer error in the browser's local extension storage. Connection reporting sends the browser name and Fetch extension version to the local application. It does not send browsing history, cookies, or download details to an analytics server.

Downloads contact the file's website. In-app update checks contact GitHub. Browser-store installation and updates contact the chosen browser store. Those services have their own privacy policies.

Users can disable capture in the extension popup, remove entries from Fetch history, or uninstall the extension. Removing a completed history entry preserves its downloaded file.

Support: https://github.com/GianCarlozxc/FetchRelease/issues

If a requested HTTP/HTTPS download is refused with HTTP 401 or 403, the extension can ask an already-open, non-private tab on the exact same origin to fetch that file using its existing browser session. Files up to 10 MB are sent to Fetch over the paired localhost connection, with their original URL and filename. This fallback runs only for a download already sent to Fetch; it does not scan unrelated pages, solve browser challenges, or accept HTML approval pages as files. If browser approval is still required, the original browser download is resumed when possible.

Torrent links and .torrent downloads explicitly sent to Fetch use its bundled BitTorrent engine. BitTorrent involves network connections to trackers, DHT bootstrap servers and peers, which can receive your IP address and torrent information. Downloading can upload pieces to peers; Fetch stops seeding after completion. Torrent filenames, paths and progress are retained locally in Fetch history. Browser cookies are not retrieved for magnet URIs.

When capture is enabled, the extension listens for genuine clicks on magnet links on HTTP/HTTPS pages, including embedded frames. It sends the clicked magnet URL and referring page to Fetch through the extension background process. It does not capture private-window links, inspect unrelated page content or trigger downloads from synthetic page clicks. Capture can be disabled in the extension popup.

For page-owned blob files, a genuine click or context-menu gesture can prepare up to 10 MB of bytes in memory on that page for up to one minute. They are sent to the paired Fetch app only when a browser download or explicit Fetch context-menu command requests them. Cross-origin blobs and private windows are excluded. Embedded data downloads are transferred over the paired localhost connection; completed history omits their contents, while paused inline jobs may retain their bytes locally for resumption.
