# 💬 Variant Chat

### Channels, DMs and badges for your Valheim server.

Keep conversations organised with chat tabs, emojis, private messages and role badges. Move chat where you want it, choose your own style and mute players when needed.

## ✨ Make yourself heard

- **💬 Channel tabs** — Local, Shout, Whisper and DM.
- **✉️ Private messages** — Click a player’s name to start a DM. Unread messages flash the DM tab.
- **😊 Emojis & mentions** — Use the smile button, or type `@` to choose an online player.
- **🛡️ Role badges** — Show a public role or a badge assigned by an admin.
- **📌 Movable chat** — Drag the title bar, pin chat open and scroll through older messages.

**Party** chat requires **Groups**. **Guild** chat requires **Guilds**.

## 📦 Install

Requires **BepInExPack Valheim 5.4.2350 or later**.

[📥 Download the latest release](https://github.com/VariantCreator/VariantChat/releases/latest)

Close Valheim, then copy `plugins/VariantChat` from the ZIP into `BepInEx/plugins/`.

**Install the same version on the server and clients.** Both players need Variant Chat to use DMs. Keep your config files when updating.

## 🚀 Get chatting

Press **Enter**, choose a channel and type.

- Click the **smile button** to pick an emoji.
- Click a **player’s name** to DM, mention or mute them.
- For mentions, type **@**, use **↑ / ↓** to choose and **Tab** to complete, or click a suggestion. Names with spaces use `@"Long Name"`.
- Drafts stay with each channel and DM while chat is open or closed.
- Click **Search** to find a player or phrase in the current tab’s recent chat. Search lasts for this session; no chat logs are saved.
- Scroll up to read older messages. **Jump to latest** returns to live chat and resumes auto-scroll.
- Drag the title bar to move the window. **Pin** keeps it visible.

## 🎨 Choose your style

Open **Style** for text size, opacity, sound and mute controls. Admins find their personal settings under **Personal**.

**Sound settings** has separate **DM** and **mention** switches, a **0–100% volume slider** and **Preview sound**. Pause alerts for **15 minutes** or **1 hour**, then resume whenever you want.

Volume sync is enabled by default. Admins can set a shared level or turn sync off so players can choose their own. **Sound switches and pauses stay personal.**

Server admins can also set the shared chat size, title and channel colours.

## 🛡️ Roles & badges

Click **Roles**, beside Style, to choose a public role or **No badge**. Viking starts green, and eight custom role slots are available.

Admins and the local host manage badges under **Style → Badges**:

- **Assign player** — Choose a player and badge, then click **Apply to [name]**.
- **Labels & colours** — Edit a role’s name, colour and Public/Hidden setting, or use **+ Add role**. Finish with **Save role settings**.

All roles start **Hidden**. Public roles appear in the player menu; hidden roles are available for admin assignment. Hiding a role keeps badges already assigned.

**Only admins can create or edit roles and assign badges to other players. Badges do not grant permissions.**

## 🧩 Config & compatibility

Settings and role lists are stored in `BepInEx/config/Variant Chat/`. Role lists accept **one SteamID64 per line**, including offline players.

Built for **Valheim 1.0.15 on Windows**, using keyboard and mouse.

**Groups, Guilds and BetterChat are optional.** Avoid running another chat UI replacement alongside Variant Chat.

---

### 📜 Credits

Code is licensed under **MIT**. [Twemoji](https://github.com/jdecked/twemoji) artwork is **CC BY 4.0**. Attribution and licenses are included in `licenses/`.
