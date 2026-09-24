# Variant Chat

A Valheim-style chat window with channel tabs, emojis, private messages and staff badges.

## Install

Requires **BepInExPack Valheim 5.4.2350** or later.

[Download the latest release](https://github.com/VariantCreator/VariantChat/releases/latest). Close Valheim, then copy the ZIP's `plugins/VariantChat` folder into `BepInEx/plugins/`.

Install the same build on the server and clients for shared settings and badges. Both players need Variant Chat for DMs. Keep your config files when updating.

## Chat

Press **Enter**, choose a channel and type. Local, Shout, Whisper and DM are included. Party needs **Groups**; Guild needs **Guilds**. Whisper is nearby chat, while DM sends to the selected player.

- Click the smile button to add emojis.
- Click a player's name to DM, mention or mute them.
- Use `@Name` or `@"Long Name"` to mention someone. Unread DMs flash the DM tab.
- Scroll up to read older messages. **Jump to latest** resumes auto-scroll.
- Drag the title bar to move the window, or use **Pin** to keep it open.

**Style** has personal opacity, optional notification sounds and mute controls. Opacity starts at **50%** and stays local. Admins open these options through **Personal**.

Server admins can also change the shared window size, chat title and channel colors. Admin controls are hidden from other players.

## Staff badges

Open **Style → Badges → Assign player**, select a player, choose **Owner**, **Admin**, **Moderator** or **No badge**, then click **Apply to [name]**.

Only the selected SteamID changes. Everyone using Variant Chat sees the badge before that player's name, such as **Owner-Dova**. Assignments save on the server and survive restarts.

**Labels & colors** changes how each role looks. **Role status** shows which players have matched the server's lists.

Badges are cosmetic. Editing them requires existing Valheim server-admin access or being the local host. Assigning an Admin badge does not grant powers or change ServerGuard permissions.

Settings are stored in `BepInEx/config/Variant Chat/`. The server also creates `owners.txt`, `admins.txt` and `moderators.txt`. You can edit these directly using one SteamID64 per line, with an optional `# name` comment. This also works for offline players. Save to reload; Owner takes priority over Admin, then Moderator.

## Compatibility

Built for Valheim **1.0.15** on Windows with keyboard and mouse. Works with BepInEx alone; Groups, Guilds and BetterChat are optional. Avoid running another chat UI replacement alongside it.

## Credits

Code: MIT. Emoji artwork: [Twemoji](https://github.com/jdecked/twemoji), by Twitter, Inc. and other contributors, under CC BY 4.0. Attribution and licenses are included in `licenses/`.
