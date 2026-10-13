# Fetch Browser Integration privacy policy

Fetch Browser Integration sends supported file downloads to the Fetch Windows application on the same computer. It has no analytics, advertising, or telemetry service.

The extension reads the download URL, suggested filename, referring page, and cookies for the specific download URL when needed to download an authenticated file. These are sent only to the paired Fetch application at 127.0.0.1 over localhost. Cookies are used in memory and are not written to Fetch download history. Fetch stores download URLs and progress in local history. Cross-origin redirects remove cookies and referrer headers.

The extension stores its local pairing token, enable/disable preference, connection details, and last transfer error in the browser's local extension storage. Connection reporting sends the browser name and Fetch extension version to the local application. It does not send browsing history, cookies, or download details to an analytics server.

Downloads contact the file's website. In-app update checks contact GitHub. Browser-store installation and updates contact the chosen browser store. Those services have their own privacy policies.

Users can disable capture in the extension popup, remove entries from Fetch history, or uninstall the extension. Removing a completed history entry preserves its downloaded file.

Support: https://github.com/GianCarlozxc/FetchRelease/issues

Torrent links and .torrent downloads explicitly sent to Fetch use its bundled BitTorrent engine. BitTorrent involves network connections to trackers, DHT bootstrap servers and peers, which can receive your IP address and torrent information. Downloading can upload pieces to peers; Fetch stops seeding after completion. Torrent filenames, paths and progress are retained locally in Fetch history. Browser cookies are not retrieved for magnet URIs.
