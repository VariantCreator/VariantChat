# Variant Chat

Chat tabs, emojis, private messages and role badges for Valheim.

## Install

Requires **BepInExPack Valheim 5.4.2350** or later.

[Download the latest release](https://github.com/VariantCreator/VariantChat/releases/latest). Close Valheim and copy `plugins/VariantChat` from the ZIP into `BepInEx/plugins/`.

Install the same version on the server and clients. Both players need the mod for DMs. Keep your config files when updating.

## Chat

Press **Enter**, choose a channel and type. Local, Shout, Whisper and DM are included. Party needs Groups; Guild needs Guilds.

- Click the smile button for emojis, or a player's name to DM, mention or mute them.
- Mention someone with `@Name` or `@"Long Name"`. Unread DMs flash the DM tab.
- Scroll up to read older messages. **Jump to latest** resumes auto-scroll.
- Drag the title bar to move chat. **Pin** keeps it visible.

## Settings

**Style** has personal opacity, sound and mute controls. Admins reach these through **Personal**.

Open **Notification volume** for the 0–100% slider and **Preview sound**. Server volume sync starts on: admins choose the shared level, or turn sync off so players can choose their own. Sound On/Off always stays personal.

Server admins can also change the shared size, title and channel colors.

## Roles

Click **Roles**, beside Style, to choose a public role or **No badge**. Viking starts green; there are eight custom role slots.

Server admins and the local host manage roles under **Style → Badges**:

- **Assign player:** choose a player and badge, then click **Apply to [name]**.
- **Labels & colors:** change a role's name, color and Public/Hidden setting, or use **+ Add role**. Click **Save role settings**.

All roles start **Hidden**. Public roles appear in the player menu; hidden roles are available for admin assignment. Hiding a role keeps badges already assigned. Only admins can create or edit roles or assign them to other players. Badges grant no permissions.

## Config and compatibility

Settings and role lists are in `BepInEx/config/Variant Chat/`. Role lists accept one SteamID64 per line, including offline players.

Built for Valheim **1.0.15** on Windows with keyboard and mouse. Groups, Guilds and BetterChat are optional. Avoid another chat UI replacement alongside it.

## Credits

Code: MIT. [Twemoji](https://github.com/jdecked/twemoji) artwork is CC BY 4.0. Attribution and licenses are in `licenses/`.
