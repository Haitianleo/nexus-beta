# NEXUS beta guide

**English · [Español](GUIA.md)**

## 1. Install

1. Download `NEXUS-Setup-….exe` from **Releases**.
2. Open it. Windows will show a blue **"Windows protected your PC"** or **"unknown publisher"** warning. That is expected: the installer is not signed yet. Click **More info** and then **Run anyway**.
3. Accept the administrator prompt. It is needed because NEXUS installs a service that reads the PC's sensors.
4. When it finishes, NEXUS opens and stays in the tray, next to the clock.

Nothing else needs to be installed.

## 2. Language

NEXUS starts in English or Spanish depending on your Windows language. You can change it at any time from the menu on the left.

## 3. First use

1. Open NEXUS and go to **Game Center**. Your Steam and Epic games appear there.
2. Open a game. With the game **closed**, press **AUTO AI** and accept.
3. You will see a spinner while it works and then a block with what it did. If there was nothing to change, it says that too.
4. **Play.** When you close the game, NEXUS waits about a minute, checks what it applied and sends a Windows notification if something changed.

The slider sets how far it goes: **MAX FPS** (look for more FPS), **BALANCED** (up to your screen's refresh rate, without stutter) or **ULTRA QUALITY** (never lowers quality).

## 4. Undo

On the game's page, **Restore everything** puts the game's settings, the NVIDIA driver and Windows back the way they were, and stops AUTO AI for that game.

## 5. Games with anti-cheat

In games with anti-cheat (for example Easy Anti-Cheat), NEXUS **only** changes the driver and Windows and does not touch the game's files. There is a permission that also lets it change that game's settings file.

**In this beta, do not turn that permission on.** It has not been tested enough, and touching a game with anti-cheat carries risks for your account that are yours alone.

## 6. What to expect

- A game's status goes from **DETECTED** to **OPTIMIZED**. "Applied" is not "optimized": NEXUS only says "optimized" once the game accepted the change and the measured FPS improved.
- If a session is short or the FPS vary a lot, NEXUS does not decide: it keeps measuring in the next one.
- NEXUS records FPS, load and temperatures while you play. That data stays on your PC.

## 7. Uninstall

**Windows Settings → Apps → NEXUS → Uninstall.** Before that, use **Restore everything** on each game where you pressed AUTO AI.

## 8. If something goes wrong

| What happens | What to try |
|---|---|
| A game does not show up | It has to be installed through Steam or Epic. Close and reopen NEXUS. |
| AUTO AI says it cannot change anything | That game stores its settings in a way NEXUS cannot write. It tells you what to change in the game's own menu. |
| The notification does not arrive | Check whether Windows has "Do not disturb" on (the bell next to the clock). |
| The game runs worse | **Restore everything** and report it in Issues. |
