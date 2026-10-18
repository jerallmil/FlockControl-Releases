# FlockControl Windows demo

Download **FlockControl.Setup.exe** from the latest release. This bootstrap downloads verified Windows x64 binaries; no Git, SDK, login or update token is required. Source is maintained separately in a private repository. This repository contains compiled distribution assets and release documentation only.

The native app and tray operate exactly four **Demo switch 1–4** mock outputs. Requested and acknowledged state are shown separately. Local control works without cloud access. No COM port or live equipment is connected. The default installer creates a Desktop shortcut but does not configure a service or automatic startup.

Optional automatic startup has a separate account/permissions review: a LocalService controller starts before login and the current user's tray starts at login. Apply only after reviewing the exact Windows changes. Service/startup behavior remains pending authorized runtime verification.

Updates check HTTPS download length and GitHub SHA-256 asset digests, then activate the app and require UI/controller readiness before committing. Settings stay outside versioned binaries. Failed candidate activation restores the prior version.

**Trust:** Publisher signing and Authenticode are not configured. Current delivery uses GitHub/HTTPS and SHA-256 integrity; it does not establish independent publisher authenticity. Windows may identify the executable as unsigned.

This is a local simulation. Physical hardware, actual phone access, and hosted dashboard delivery are not verified. The service executable is a reviewed optional installer component, not a file to launch or register manually.