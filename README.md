# lingo-config

Public settings for the Lingo app. Keep this repository **public**, and never rename or delete it
(or the GitHub account): every installed app reads it.

## server.json — where the app finds its server

```json
{ "apiBaseUrl": "http://lingolang.runasp.net/" }
```

The app reads this file every time it starts. It switches to a new address only when that
server answers `api/health` with `"status":"healthy"`, so a wrong address cannot break the app.
After you change it, phones move on their next start (GitHub may cache the file for up to ~10 minutes).

Edit it on github.com: open `server.json` → pencil icon → change the address → **Commit changes**.

## privacy.html — privacy policy

Public link for Google Play: https://mohamedbadawi16.github.io/lingo-config/privacy.html
