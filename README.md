# NEXUS AI Ecosystem — closed beta

**English · [Español](README.es.md)**

NEXUS is a Windows program that tunes your games' graphics **on its own, by measuring**: it tries one change, watches how your FPS actually move while you play, and keeps only what really helps on your PC.

> **This is a beta.** It has been tested on very few machines. It may fail. Everything it changes can be undone with one button.

The app is available in **English and Spanish**. It picks the language of your Windows the first time, and you can switch it at any moment from the menu.

## What it does

- **AUTO AI:** press one button on a game and NEXUS studies its files, applies what it can safely change and, after each session, checks the result and carries on by itself.
- **It measures for real:** no promised FPS. It compares what it measured before and after and tells you, also when a change did not help.
- **Three routes:** the game's own settings, the NVIDIA driver and the Windows graphics settings.
- **Restore everything:** one button puts every setting back the way it was.
- **A Windows notification** when something changes after a session.
- Also: live PC dashboard (temperatures, load, FPS), your Steam and Epic library, and power controls.

## What it does not do

- It does not modify game executables or data packages.
- It does not touch, disable or bypass anti-cheat systems.
- It does not decrypt protected files: if a game encrypts its settings, NEXUS says so and uses other routes.
- It does not make numbers up: what it cannot measure is shown as "—".

## Requirements

- Windows 11 (64-bit).
- An NVIDIA graphics card to get the most out of it. With AMD or Intel the dashboard and the game-file route work, but they are less tested.
- Games from Steam or Epic. Automatic optimisation is built for Unreal Engine games; with other engines it does less.

## Download

Go to **[Releases](../../releases)** and download `NEXUS-Setup-….exe`.

Read the **[installation guide](GUIDE.md)** first: it explains the Windows "unknown publisher" warning and how to undo everything.

## Coming soon

- **Phone app (iPhone and Android):** see your PC, launch AUTO AI and turn the PC on or off from your phone. It already works in internal testing; there is no release date yet.
- **Signed installer**, so Windows stops showing the "unknown publisher" warning.

No dates are promised: things are released when they have been tested.

## Tested so far

| Game | Result |
|---|---|
| Phantom Blade Zero | Ray tracing turned off from outside the game: from 67 to 81 FPS on average (RTX 3080, 4K), measured and confirmed by the game itself |
| SILENT HILL: Townfall | Settings applied; measurement pending |
| Halloween: The Game | Driver and Windows applied; measurement pending |

These are results from a single PC. Yours may differ: that is what the beta is for.

## Tell me how it went

Use the **Feedback & support** button inside NEXUS, or open an entry in **[Issues](../../issues)** with:

1. Your graphics card and processor.
2. The game.
3. What NEXUS showed after you played (a screenshot of the "AUTO AI · result" block is enough).
4. What you expected and what happened.

## Support the project

NEXUS is free during the beta and is made by one person. If you find it useful, you can support it on **[Ko-fi](https://ko-fi.com/12thmonth)**.

Contributions go to two specific things:

- **The phone app on the App Store.** Publishing there requires a paid Apple developer account every year. It is the app to see your PC, launch AUTO AI and play your games from your phone, also away from home.
- **Signing the Windows installer**, so the "unknown publisher" warning goes away. The certificate is also paid.

Supporting does not unlock anything different and does not buy a date: the beta is the same for everyone.

## Licence

NEXUS is proprietary software. This beta is offered for testing only: see **[LICENSE.md](LICENSE.md)**. It ships with third-party components under their own licences: **[TERCEROS.md](TERCEROS.md)**.
