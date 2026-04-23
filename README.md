# Outer Worlds 2 - Item ID Database

A searchable directory of 1,787 Outer Worlds 2 blueprint item IDs for use with console commands. Search by name, filter by category, click any item to see its full details and copy the blueprint ID.

**Live at:** [ow2.opensourceforall.com](https://ow2.opensourceforall.com)

## How to Use

1. Go to the site
2. Type in the search bar to filter by item name, brand, or variant
3. Use the category buttons to narrow results (Weapons, Armor, Items, Pets, Traits, Throwables)
4. Click any item to open a detail card
5. Copy the blueprint ID
6. Paste it in the game console

## Features

- Instant search across all 1,787 items
- Category filters: Weapons (213), Armor (501), Items (1000), Pets (41), Traits (25), Throwables (7)
- Click any item to open a detail card showing blueprint ID, full asset path, faction/brand, and variant type
- One-click copy to clipboard for console commands
- Detects item metadata from asset paths including faction (Protectorate, SubRosa, AuntiesChoice, Scrappers, ChosenFleet, EarthDirectorate, etc.) and variant type (Base, Modded, Unique, Rift, Boss)
- Items grouped under subcategory headers (Weapons - AR, Armor - BodyArmor, Items - Consumable, etc.)
- Mobile responsive
- Dark sci-fi terminal UI

## Data Categories

| Category | Count | Examples |
|----------|-------|---------|
| Weapons | 213 | Assault Rifles, LMGs, Melee, Pistols, Shotguns, SMGs, Snipers, Launchers, Specials |
| Armor | 501 | Body Armor, Headgear, Undersuits, CryoSuits |
| Items | 1000 | Consumables, Crafting, Collectibles, Junk, Audio Logs, Gadgets, Inhalers, Loot Tables |
| Pets | 41 | Bred Worms, Critters, Companions |
| Traits | 25 | Character and Companion Traits |
| Throwables | 7 | Explosive Grenades |

## Technical Details

The site is a single-file static HTML page with no external dependencies beyond Google Fonts. All 1,787 items are embedded in the page and filtered client-side for instant results. No backend, no API calls, no loading times.

The GitHub Actions pipeline (`build.yml`) extracts item data from a password-protected RAR archive containing categorized .txt files, parses them with `parse_rar.py`, and injects the generated data into both `index.html` and `item_directory.html`.

## Credit

Original item data extraction and GitHub Actions pipeline by [Pacmanninja](https://github.com/Pacmanninja/outerworld2-Item-IDs). This fork is a full UI rebuild by [OpenSourcePatents](https://github.com/OpenSourcePatents).

All original files (`item_directory.html`, `parse_rar.py`, workflows) are preserved. The build pipeline injects data into both `index.html` and `item_directory.html`.

---

## Original Project

### Access the original at: [https://pacmanninja.github.io/outerworld2-Item-IDs/](https://pacmanninja.github.io/outerworld2-Item-IDs/)

Report IDs that don't work [here in this issue](https://github.com/Pacmanninja/outerworld2-Item-IDs/issues/1)

### Little hint:

![Alt text](hint.png)

---

## License

MIT (inherited from original repo)
