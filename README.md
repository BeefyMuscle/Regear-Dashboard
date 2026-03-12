# ⚔ Regear Dashboard

A real-time guild inventory tracker for Albion Online. Track your T7/T8/T9 gear stock across every armor type and weapon tree, coordinate crafting, and keep your whole officer team in sync — live.

Made by **BeefyMuscle** using Claude Sonnet 4.6.

---

## Getting Started

On your **first visit** you'll be asked for your **in-game name**. This is shown to guildmates in the who's online list so everyone knows who's making changes. You can update it anytime by clicking the online pill in the top bar.

After that you'll be asked to either **create** or **join** a room:

- **Creating a room** — enter your guild name and set a password. You'll get an 8-character room code to share with your officers.
- **Joining a room** — enter the room code and password your guild leader gave you.

Once you're in, all changes sync in real time. Anyone in the room sees updates as they happen.

---

## Tracking Inventory

Browse the **Tier 7, Tier 8, and Tier 9** tabs to see every tracked item. Use the category buttons at the top of each tab to jump to a specific type — helmets, jackets, shoes, offhands, or a weapon tree.

- **Have** — how many of this item you currently have in stock. Hit `+` / `−` to adjust, or **Shift+click** to move by 10 at a time.
- **Par** — your target quantity. Set this to whatever your guild wants to keep on hand.
- **Need** — calculated automatically. Rows highlighted red are below par.

Click any column header (**Have**, **Par**, **Need**) to sort — click again to reverse.

---

## Flags

Each item has two optional flags you can toggle:

- **★ PRI** (purple) — marks an item as priority. It gets a purple border and rises to the top of the Priority Shortages list on the Summary tab.
- **✕ IGN** (amber) — marks an item as ignored. It will be excluded from the Assignment tab and Order Sheet even when below par. Use this for items your guild doesn't craft.

---

## Assignment & Order Sheet

The **Assignment** tab is your active crafting to-do list. It shows every item that is below par and not ignored, sorted with priority items first, then by highest need count.

Click a crafter's name tag under any item to **assign** it to them — click again to unassign. Assignments carry through to the Order Sheet and the exported file.

The **Order Sheet** shows the same list in a cleaner format with material quantities pre-calculated per item. Hit **Fulfill Order** on any item to set its Have count to par — it disappears from the sheet immediately and syncs to everyone in the room.

Click **Export .txt** on the Order Sheet to download a formatted text file — useful for dropping in Discord or handing off to crafters. The export includes:

- All orders with required materials per item
- Royal gear entries additionally list the required **Miscellaneous Sigils**
- A **Total Materials** breakdown by tier
- An **Expected Return (15%)** section showing base materials you can expect back from the crafting return rate

---

## Crafters

On the **Crafters** tab you can add player names under each crafting specialisation — grouped by armor type and weapon tree.

Once added, a crafter's name appears as a clickable tag under relevant items on the Assignment tab. Click a tag to assign that item to them, click again to unassign. Removing a crafter automatically clears all their assignments across all items.

---

## Summary

The **Summary** tab gives you a bird's-eye view of your guild's readiness — overall stocked percentage, a Craft Queue count (items below par and not ignored), per-tier breakdowns, and a priority shortages list of everything flagged PRI that you're still short on.

---

## Edit Mode

Click **✎ Edit Items** in the tab bar to enter Edit Mode. This reveals two extra tools:

- **Hide toggle** — remove items your guild doesn't use. Hidden items are excluded from all counts, need calculations, and order sheets. They show as faded striped rows in Edit Mode so you can always re-enable them.
- **Bulk par setter** — set par for the current category, the whole tier, or all tiers at once in one click. Skips hidden items.

---

## Room Settings

Click **⚙ Settings** in the top bar to:

- Rename your guild room
- Change the room password
- Reset all inventory counts to zero (syncs to everyone immediately — use with care)

---

## Who's Online

The green pill in the top bar shows how many officers are currently viewing the room. Click it to see their names and update your own display name.

---

## Stale Data Warning

If a room hasn't been updated in over 30 days, you'll see an amber warning banner when you join. It's a reminder to double-check the numbers are still current before a big operation.

---

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `1` | Summary |
| `2` | Tier 7 |
| `3` | Tier 8 |
| `4` | Tier 9 |
| `5` | Assignment |
| `6` | Order Sheet |
| `7` | Crafters |
| `E` | Toggle Edit Mode |
| `D` | Toggle dark mode |
