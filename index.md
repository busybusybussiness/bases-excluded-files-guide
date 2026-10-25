# Bases and excluded files: what works today (honest guide)

**Last checked:** 2026-10-24 against the live pages linked below. Not affiliated with Obsidian. No sponsorship, no affiliate links.

## The problem
In Obsidian, putting a folder under **Settings → Files and links → Excluded files** keeps its notes out of Quick Switcher and link suggestions. In the forum thread where users reported it, the same exclusion also removes those notes from **Bases** views, so a Base built on that folder shows nothing ([bug-graveyard thread](https://forum.obsidian.md/t/excluding-folders-from-quick-switcher-also-excludes-them-from-bases/110121)). A moderator reply in that thread says this is how it currently works, not a bug.

Users have asked for a per-Base toggle to include excluded files since mid-2025 ([feature request](https://forum.obsidian.md/t/bases-toggle-to-show-excluded-files/102378)). As of the latest reply in that thread (October 2026), no native toggle has been added.

**Status, as of 2026-10-24:** FACT. There is no native toggle. The thread says the Bases option is still a request.

## Option 1: a community plugin (third party)
A community plugin named **Toggle Excluded Folders** exists. Its author posted it in the feature-request thread and it is listed on GitHub:
https://github.com/ssurfthekaliyuga/obsidian-toggle-excluded-folders (version 1.0.2, last commit 2026-05-27; its license was not checked by us).

- It is a third-party plugin. Install it only from Obsidian's community plugin browser, and read its code or permissions before enabling it.
- **Not tested by us.** We have not installed it in the Obsidian app. Whether it does exactly what you need is UNKNOWN until you test it on a copy of your vault.

## Option 2: a property filter (untested in the app)
You can avoid the exclusion problem altogether by not excluding the folder. Instead, mark the notes you want hidden from the Base with a frontmatter property, for example `hide: true`, and add a filter to the Base view.

- The Bases filter syntax is documented at https://obsidian.md/help/bases/syntax (a base includes every file in the vault by default, and filters narrow it).
- Whether this works the way you want in your own Obsidian version is UNKNOWN until you test it.
- This option does not hide the notes from Quick Switcher. It only changes what the Base shows.

## How to test safely (5 minutes)
1. Back up your vault or use a copy.
2. Pick one folder you want excluded and create one Base on it.
3. Try Option 2 first (no plugin). If it works, you are done.
4. If you need Quick Switcher to ignore those notes too, install Option 1 on the copy and check the Base again.
5. Only then change your real vault.

## What we do not know
- Whether Option 1 works on your Obsidian version (not tested by us).
- Whether Option 2 behaves as expected in every view type (not tested in the app).
- How many people use either workaround (no public data).

If you test either option and it works or fails, tell us in the feature-request thread or open a GitHub issue. We will update this page with what you report, dated and labelled.

## Sources (all checked live 2026-10-24)
- https://forum.obsidian.md/t/excluding-folders-from-quick-switcher-also-excludes-them-from-bases/110121
- https://forum.obsidian.md/t/bases-toggle-to-show-excluded-files/102378
- https://github.com/ssurfthekaliyuga/obsidian-toggle-excluded-folders
- https://obsidian.md/help/bases/syntax
