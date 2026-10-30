# Sources and extensions

Nekomo uses external sources and extension ecosystems. Sources are independently maintained and may change without Nekomo releases.

1. Find the source through its official developer or project channel.
2. Confirm its ecosystem, version requirements, and compatibility with your Nekomo build.
3. Review permissions and publisher information.
4. Follow the source's installation and update instructions.
5. Test it and report reproducible issues with version details.

Nekomo does not host or bundle third-party extension packages. Never share login credentials, session cookies, or API tokens in support requests.

See [Nekomo Extensions](https://github.com/Nekomo-App/Nekomo-Extensions) for format-specific notes and compatibility reports.

## The optional Nekomo repository and the Extensions manager

Nekomo ships with no sources installed. Open **Settings > Extensions** to reach the Extensions manager, one place for:

- **Repositories and sources:** CloudStream plugins (`.cs3`) and Zangetsu scripts (`.js`). Enable, disable, update, uninstall, view details and per-provider switches.
- **Metadata APIs (built in):** AniList (main), Kitsu, MyAnimeList via Jikan, TVMaze and TMDB (needs your own key). Backups switch on automatically when the main API is down or rate-limited.
- **Automatic updates:** on or off, frequency (6 hours to 7 days), manual check, update all or one by one, and an update history that records every install, update, removal and error. A failed update keeps the previous version.
- **APK extensions (Aniyomi, Mihon):** listed separately. Nekomo never downloads, installs or updates these automatically; you install them yourself.

An **optional official repository** (free and legal sources only) can be added from the same screen with a repository URL or code. Nothing is installed until you add it and confirm the third-party-code warning, and you can remove it, with the sources it installed, at any time. Any other repository can be added manually by URL; Nekomo does not host or vouch for those.

## NEX, the companion manager

[NEX](https://github.com/Nekomo-App/NEX) (Nekomo Extension Exchange) is a separate app from the Nekomo community that manages repositories, extensions and sources for Nekomo, Mihon, Aniyomi, CloudStream and Zangetsu. It ships with no repositories, hosts nothing, and never installs silently. From NEX you can send a repository to Nekomo with one tap (Nekomo asks you to confirm), check Nekomo app updates with SHA-256 verification, and keep Mihon and Aniyomi extensions up to date. Downloads are on its [releases page](https://github.com/Nekomo-App/NEX/releases).
