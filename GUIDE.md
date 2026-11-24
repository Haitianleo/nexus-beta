# NEXUS beta guide

**English · [Español](GUIA.md)**

## 1. Install

1. Download `NEXUS-Setup-….exe` from **Releases**.
2. Open it. Windows will show a blue **"Windows protected your PC"** or **"unknown publisher"** warning. That is expected: the installer is not signed yet. Click **More info** and then **Run anyway**. (If Windows has *Smart App Control* turned on, it blocks unsigned apps, NEXUS included.)
3. Accept the administrator prompt. It is needed because NEXUS installs a service that reads the PC's sensors.
4. When it finishes, NEXUS opens and stays in the tray, next to the clock.

Nothing else needs to be installed. If you already have 0.39, you don't need to download anything: NEXUS offers the new version by itself, with **Update now**.

The first time it opens, a notice explains the anonymous statistics. They come turned on, and you can turn them off right there or later in **Connection & security → Privacy**.

## 2. Language

NEXUS starts in English or Spanish depending on your Windows language. You can change it at any time from the menu on the left.

## 3. First use

1. Open NEXUS and go to **Game Center**. Your games from Steam, Epic Games, Xbox (Xbox app, PC Game Pass and Microsoft Store), GOG, Ubisoft Connect, EA app, Amazon Games and Riot Games appear there. Each card shows its launcher, and you can filter the list by launcher.
2. A game from somewhere else (Battle.net, an emulator, a standalone game)? Press **Add a game** and pick its `.exe`.
3. Open a game. With the game **closed**, press **AUTO AI · let NEXUS do it** and confirm.
4. You will see a spinner while it works and then a block with what it did. If there was nothing to change, it says that too.
5. **Play.** When you close the game, NEXUS waits about a minute and checks what it applied. The result is on the game's page, and when a change measurably raised your FPS a Windows notification tells you.

The slider sets how far it goes: **MAX FPS** (look for more FPS), **BALANCED** (up to your screen's refresh rate, without stutter) or **ULTRA QUALITY** (never lowers quality). In **FPS target** you can also type your own number for that game, for example 90.

After your first measured session NEXUS asks, once, whether this version works better, the same or worse for you than the last one. You can close it without answering.

## 4. Settings guide

It measures what each setting costs on your PC, one at a time, and lets you choose.

1. On the game's page, find **Settings guide** and press **Start the guide**.
2. Play a normal session and close the game. That is the reference.
3. NEXUS lowers one setting one level. Play another session and close the game: NEXUS measures it, puts the setting back and moves on to the next one. Each result appears in the guide's table.
4. After the game's own settings it also tries a few graphics driver and Windows options (for example, Windows' optimizations for windowed games). They don't touch the game's files, so the guide can test them in games with anti-cheat too.
5. When it finishes, tick the settings that are worth it to you and press **Apply selected**. **Restore everything** undoes it.

Tips: play in similar areas in every session, and don't change graphics in the game's menu while the guide runs. AUTO AI waits until the guide is finished. **Stop guide** ends it at any moment; whatever was on trial goes back the way it was.

## 5. Undo

On the game's page, **Restore everything** puts the game's settings, the graphics driver and Windows back the way they were, and stops AUTO AI for that game.

## 6. Games with anti-cheat

In games where NEXUS knows there is an anti-cheat (Easy Anti-Cheat, BattlEye, Riot Vanguard, NCGuard and others), it **only** changes the graphics driver and Windows and does not touch the game's files.

When you press **AUTO AI · let NEXUS do it** on one of those games, the window tells you so and shows **Extend permissions (optional, at your own risk)** with two boxes, both unticked:

1. **The game's settings file**: the same file the game's own graphics menu writes.
2. **Engine.ini**: it can change things the menu doesn't allow, like fog. In an online game that may be seen as cheating. If you tick it, NEXUS shows a warning and asks again (**I understand the risk**).

**In this beta, leave both unticked in online games.** If you turn them on, the risk to your account is yours alone. **Remove permissions**, on the game's page, takes them back and puts back what was changed with them.

If NEXUS learns that a game uses anti-cheat after it had already changed something, it undoes nothing on its own: it tells you and changes nothing else in the game's files without your permission.

## 7. Graphics cards

- **NVIDIA:** full support.
- **Intel:** temperature, fan and driver settings; new and not yet tested on real Intel cards.
- **AMD:** temperature, fan and power draw; driver settings arrive in a coming version.

With any card NEXUS can change the game's own settings and Windows' graphics options for that game, and it measures your FPS the same way.

**Have an AMD or Intel card?** That support is new and I have no such card to test with. Help me by sending the diagnostics: **Connection & security → Help → Export diagnostics** saves a `.zip` (no user name, no PC name, no full paths; NEXUS never sends it). Attach it to an entry in [Issues](../../issues) and say which card you have. **GitHub Issues are public: attaching the `.zip` there publishes it.** The file names your games, so have a look inside first.

## 8. What to expect

- A game's status goes from **DETECTED** to **OPTIMIZED**. "Applied" is not "optimized": NEXUS only says "optimized" once the game accepted the change and the measured FPS improved.
- If a session is short or the FPS vary a lot, NEXUS does not decide: it keeps measuring in the next one.
- NEXUS records FPS, load and temperatures while you play. That data stays on your PC.

## 9. Uninstall

**Windows Settings → Apps → NEXUS → Uninstall.** Before that, use **Restore everything** on each game where you pressed AUTO AI.

## 10. If something goes wrong

| What happens | What to try |
|---|---|
| A game does not show up | Press **Add a game** in Game Center and pick the game's `.exe`. If it comes from one of the launchers in section 3, tell me: several of them are new in 0.40 and not tried with real games yet. |
| AUTO AI says it cannot change anything | That game stores its settings in a way NEXUS cannot write. It tells you what to change in the game's own menu. |
| The notification does not arrive | Check whether Windows has "Do not disturb" on (the bell next to the clock), and that this kind of notification is on in **Connection & security → Windows notifications**. |
| The game runs worse | **Restore everything** and tell me in the [feedback form](https://forms.gle/orRMRurHcRCdbiBRA) (no account needed) or in Issues. |
| Something looks wrong with an AMD or Intel card | **Restore everything** undoes what NEXUS changed. Then send me **Export diagnostics** (section 7). |
