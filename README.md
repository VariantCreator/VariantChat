# Variant Chat

A Valheim-style chat window with channel tabs, emojis, private messages and custom role badges.

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

## Display roles

Open **Style → Badges → Assign player**, select a player, open the badge selector and choose **Owner**, **Admin**, **Moderator**, **Viking**, a custom role or **No badge**. Click **Apply to [name]**. Scroll the selector to see more roles.

Only the selected SteamID changes. Everyone using Variant Chat sees the badge before that player's name, such as **Owner-Dova**. Assignments save on the server and survive restarts.

**Viking** starts green. **Labels & colors** changes each role's name, color and visibility. Admins can use **+ Add role** to create up to eight custom roles, then click **Save role settings**. **Role status** shows which players have matched the server's lists.

Only Valheim server admins and the local host can create or edit roles and assign them to other players. Badges are cosmetic: an Owner, Admin or Moderator badge grants no powers and does not change ServerGuard permissions. Each player has one display badge.

### Public and hidden roles

Players click **Roles**, beside **Style**, to choose a public role or **No badge**. This changes only their own badge and saves on the server.

Admins open **Style → Badges → Labels & colors**, choose a role with the arrows, and click its visibility button to switch between **Public** and **Hidden**. Click **Save role settings** to apply it. Public roles appear in the player menu; hidden roles remain available for admin assignment. Every role starts hidden until you make it public, including Viking and new custom roles.

Hiding a role removes it from the player menu immediately. It does not remove badges already assigned to players. Use **Assign player** to change or remove those badges. Role creation and visibility controls remain admin-only.

Settings are stored in `BepInEx/config/Variant Chat/`. The server creates `owners.txt`, `admins.txt`, `moderators.txt`, `vikings.txt` and `custom1.txt` through `custom8.txt`. You can edit these directly using one SteamID64 per line, with an optional `# name` comment. This also works for offline players. Save to reload. If an account appears in several lists, priority is Owner, Admin, Moderator, Viking, then custom roles in slot order.

Custom role names, colors and Public settings are saved in the server config under **Badges**. An empty custom label disables that role while retaining its saved assignments. Use 1.0.5 or later on the server and clients for player role selection. Older clients keep the badges their version supports.

## Compatibility

Built for Valheim **1.0.15** on Windows with keyboard and mouse. Works with BepInEx alone; Groups, Guilds and BetterChat are optional. Avoid running another chat UI replacement alongside it.

## Credits

Code: MIT. Emoji artwork: [Twemoji](https://github.com/jdecked/twemoji), by Twitter, Inc. and other contributors, under CC BY 4.0. Attribution and licenses are included in `licenses/`.
