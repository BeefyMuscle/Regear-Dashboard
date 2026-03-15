# Regear Dashboard v1.5.0

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

Browse the **Tier 7, Tier 8, and Tier 9** tabs to see every tracked item. Use the **category filter bar** at the top to jump to a specific type — helmets, jackets, shoes, offhands, or a weapon tree. Use the **search box** on the right of the filter bar to find a specific item by name.

- **Have** — how many of this item you currently have in stock. Hit `+` / `−` to adjust, or **Shift+click** to move by 10 at a time.
- **Par** — your target quantity. Set this to whatever your guild wants to keep on hand.
- **Need** — calculated automatically. Rows highlighted red are below par.
- **Note** — a short text field for reminders like "waiting on artefacts". Notes show in amber and are visible on the Order Sheet.

Click any column header (**Have**, **Par**, **Need**) to sort — click again to reverse.

---

## Rapid Entry

Click **Rapid Entry** in the tab bar (or press `R`) to open a fullscreen wheel for quickly entering chest counts. It opens on whichever tier you're currently viewing.

Scroll through items with `↑`/`↓` arrow keys or `W`/`S`. The active item sits large and centred — type a number directly into the input. Press `W`/`S` while the input is focused to commit the value and move to the next item immediately.

Hidden items are skipped. Press `R` to save and close, or `Esc` to discard all changes.

---

## Flags

Each item has two optional flags:

- **★ PRI** (purple) — marks an item as priority. It gets a purple border, rises to the top of Priority Shortages on the Summary tab, and sorts first on the Assignment and Order Sheet.
- **✕ IGN** (amber) — marks an item as ignored. It will be excluded from the Assignment tab and Order Sheet even when below par. Use this for items your guild doesn't craft.

---

## Assignment & Order Sheet

Both tabs have a **category filter bar** to narrow the list. Filters are independent of each other and of the tier tab filters.

The **Assignment** tab is your live crafting to-do list — every item below par and not ignored, sorted with priority items first then by highest need. Click a crafter's name tag to assign an item to them, click again to unassign.

The **Order Sheet** shows the same list with material quantities pre-calculated. Click **Fulfill Order** on any item — the button turns amber to confirm. On confirm, Have is set to par and the change syncs to everyone instantly.

Click **Export .txt** to download a formatted text file with all orders, a **Total Materials** breakdown by tier, and an **Expected Return (15%)** section. Royal gear additionally lists the required Miscellaneous Sigils.

---

## Crafters

On the **Crafters** tab you can add player names under each crafting specialisation — grouped by armor type and weapon tree. Each crafter only appears as a tag under items they can actually craft, not across all categories.

Removing a crafter automatically clears all their assignments across all items.

---

## Change Log

The **Log** tab records every Have, Par, flag, note, and Fulfill change — who made it, what changed, and when. Keeps up to 100 entries, newest first.

Rapid consecutive changes to the same item collapse into a single entry. Officers can clear the log from the Log tab. Crafters can view but not clear it.

---

## Summary

The **Summary** tab gives you a bird's-eye view of your guild's readiness — overall stocked percentage, a Craft Queue count, per-tier breakdowns, and a scrollable Priority Shortages list of everything flagged PRI that you're still short on.

---

## Edit Mode

Click **✎ Edit Items** in the tab bar to enter Edit Mode. This reveals two extra tools:

- **Hide toggle** — remove items your guild doesn't use. Hidden items are excluded from all counts, need calculations, and order sheets. They show as faded striped rows in Edit Mode so you can always re-enable them.
- **Bulk par setter** — set par for the current category, the whole tier, or all tiers at once in one click. Skips hidden items.

---

## Crafter Access

Officers can set a separate **Crafter Password** in Settings. Share the room code and crafter password with your crafters — they join the same room but with a restricted view.

Crafters can see **Summary**, **Assignment**, and **Order Sheet**. They can hit **Fulfill Order** to mark items done, but cannot edit Have/Par, toggle flags, manage the crafters list, access Settings, or change assignments. A **Crafter View** badge appears in their nav so the mode is always clear.

---

## Room Settings

Click **Settings** in the top bar to:

- Rename your guild room
- Change the officer or crafter password
- Reset all inventory counts to zero (syncs to everyone immediately — use with care)
- Restore a backup

**Backups** are saved automatically each time you load the room — the last 3 snapshots are kept. Restoring one overwrites current data and syncs to everyone in the room immediately.

---

## Who's Online

The green pill in the top bar shows how many members are currently viewing the room. Click it to see their names and update your own display name.

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
| `8` | Log |
| `R` | Open / save & close Rapid Entry |
| `E` | Toggle Edit Mode (on tier tabs) |
| `D` | Toggle dark mode |
| `↑↓` / `W S` | Navigate Rapid Entry wheel |
| `Esc` | Discard and close Rapid Entry |
