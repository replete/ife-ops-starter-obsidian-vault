# Obsidian CSS snippets for Minimal Theme

![Screenshot](screenshots/screenshot.png)

My working folder of CSS snippets for Obsidian configured with the [Minimal Theme](https://github.com/kepano/obsidian-minimal). The purpose is to extend Obsidian UI possibilities and also visually harmonize the style of various plugins with `Minimal Theme`, with a preference for compact UI. Updated regularly. Screenshots below. Some snippets will probably work fine on default or other themes.

## How to use

1. Clone/[fork](https://github.com/replete/obsidian-minimal-theme-css-snippets/fork)/[unzip](https://github.com/replete/obsidian-minimal-theme-css-snippets/archive/refs/heads/main.zip) into `<your vault location>/.obsidian/snippets` or use 'Snippet Downloader' plugin
2. (recommended) Install the [MySnippets plugin](https://github.com/chetachiezikeuzor/MySnippets-Plugin) via 'Community plugins' to easily manage snippets    
![MySnippets plugin screenshot](screenshots/mysnippets.png)
4. Check periodically for updates and new goodies

## Support development


<a href="https://www.buymeacoffee.com/replete"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=replete&button_colour=BD5FFF&font_colour=ffffff&font_family=Poppins&outline_colour=000000&coffee_colour=FFDD00" /></a>


## Updates (scroll to next section for snippet details)
- **2024-04-09** Make.MD banners broke for me again. Might be a conflict of some kind. I've submitted an [issue on their github](https://github.com/Make-md/makemd/issues/297) so chip in if you also have the same problem.
- **2024-03-20** Make.MD Banners are back. Thankfully they've sorted out whatever was going on, so I've refactored the snippets entirely, and it works much better with less code.
- **2024-03-17** Added new Omnisearch plugin visual fixes. I've made a number of changes in recent commits but haven't updated notes. At some point I'll update screenshots and things.
- **2024-02-21** Disabled a number of plugins for performance reasons. Trying out ollama embeddings plugin, but its early days.
- **2024-02-21** Works on mobile. Make.MD banners stopped working again, combined with the broken inline file context I've chosen to just give up and disable Make.MD for now. I'll live without the pretty banners, it's a shame to lose this nice functionality but there are no other banner plugin alternatives that work and Make.MD is no longer worth dealing with. I'll leave the banner functionality here but if it works for you now, updating it may cause you problems.
- **2024-02-08**: Make.MD's inline context (filename in editor) has broken for a while, I've refactored CSS and reinstalled Make.MD but ths bug remains, so for some new files the inline context filename does not show. Reinstalling Make.MD did make my banner show again however and I've fixed the CSS for it. If you have problems, try uninstalling and reinstalling the plugin and reseting the options (disable everything but `Sync Context Fields..., Flow (beta), Inline Context, Flow Block, Open Flow Blocks...` if you wish to replicate my setup, which these snippets are configured for). I only use Make.MD for the banner functionality as there's no other option right now, and look forward to getting rid of this plugin entirely in the future.

## My environment

- `MacOS 13.6.5`, `Android 13`
- `Obsidian v1.5.12 (installer 1.5.11)` Desktop, if installer < 1.1.8 reinstall from official installer to update electron for updated CSS features like `:has()` - homebrew update didn't work for this version)
- `Minimal Theme v7.5.4`
```js
// plugins I currently have enabled (36):
['obsidian-advanced-uri', 'auto-class', 'calendar', 'cmdr', 'obsidian-hide-sidebars-when-narrow', 'hotkeysplus-obsidian', 'obsidian-icon-folder', 'obsidian-excalidraw-plugin', 'cm-editor-syntax-highlight-obsidian', 'obsidian-minimal-settings', 'obsidian-meta-bind-plugin', 'open-vscode', 'periodic-notes', 'quickadd', 'obsidian-task-progress-bar', 'templater-obsidian', 'obsidian-toggle-list', 'mysnippets-plugin', 'no-dupe-leaves', 'file-explorer-note-count', 'easy-toggle-sidebars', 'settings-search', 'modalforms', 'obsidian-daily-note-outline', 'custom-sort', 'obsidian-shortcut-launcher', 'obsidian-contextual-typography', 'open-in-new-tab', 'obsidian-tracker', 'omnisearch', 'snippet-commands-obsidian', 'dataview', 'obsidian-custom-frames', 'make-md', 'meld-encrypt', 'obsidian-static-file-server']
// [...new Set(app.plugins.enabledPlugins)]
```

> ⭐ A star beside the follow snippet titles indicate I have it enabled in my vault (and should work well for you too as a default configuration)
## Editor Snippets
- **Custom Tag Styles** ⭐ - I'm not using tags much at the moment, but prefer the more compact look than the pill shaped. If I use tags more I'll extend this.
    ![Custom tag styles screenshot](screenshots/custom-tags.png)
- **Compact Right Sidebar notes** ⭐ - This shortens the margins and enables a duotone when not hovering for when a note is open in the right panel workspace (reading view atm)
- **Editor fixes** ⭐ - gutter component alignments, general editor fixes, less visible indentation guide
- **Frontmatter tweaks** ⭐ - styling, fixes for `editor syntax highlighter plugin`
- **Table tweaks** ⭐ - WIP, still waiting for a good table editing plugin...
- **Top Fade** - Remove harsh edge of content when using "Compact Tabs (classic)" with one of the positional Tab Header snippets (I prefer the Translucent Tab Header)
![Top fade screenshot](screenshots/top-fade.png)
- **Typography fixes** ⭐ - alignment fixes for editor, headings, list items quotes etc (WIP)
    ![Typography fixes](screenshots/typography-fixes.png)
## Font snippets:
- **Mono Emojis** - embedded Noto Emoji variable font (2MB snippet!) - not recommended
## UI snippets:
- **Collapsible Right Headers** ⭐ - Hide panel headers until hover in the right sidebar.
    ![Collapsible right headers screenshot](screenshots/collapsible-header.gif)
- **Compact File Explorer** ⭐ - Compact styles, chevrons on right, makes attachment folders less visible    
    ![Compact File Explorer screenshot](screenshots/compact-file-explorer.png)    
- **Compact Properties (+autohide)** ⭐ - Compact Properties (Obsidian 1.4.5 feature) with hover autohide, just like the Make.MD snippet [note: I keep the Make.MD + snippets enabled for the banner functionality]
    ![Compact Properties screenshot](screenshots/compact-properties.gif)
- **Compact Tab Header** ⭐ - Compact icons in toolbar, also fixes `Commander` plugin icon colours    
- **Compact Sidebar Header** ⭐ - Make main tab header items more compact
    ![Compact Tab Header screenshot](screenshots/compact-tab-header.png)
- **Compact Tabs** ⭐ - Compact firefox-style pill tabs, better for smaller screens     
    ![Compact Tabs screenshot](screenshots/compact-tabs.png)
- **Compact Tabs (classic)** - Compact classic tabs, better for smaller screens    
    ![Compact Tabs classic screenshot](screenshots/compact-tabs-classic.png)
- **Custom Separators** ⭐ - user-configurable CSS for separators, works well with `File Explorer Custom Sorting` plugin    
    ![Custom Separator screenshot](screenshots/custom-separators.png)
- **Custom Separators (gradient)** - user-configurable CSS for separators, works well with `File Explorer Custom Sorting` plugin    
    ![Custom Separators (gradient) screenshot](screenshots/custom-separators-gradient.png)
- **Floating Tab Header** - Save space with this float right leaf tab header (show navigation, breadcrumb on hover/focus)    
    ![Floating Tab Header screenshot](screenshots/floating-tab-header.gif)
- **Floating Tab Header (mini)** - Save even more space with this float right leaf tab header (show navigation, breadcrumb on hover/focus)    
    ![Floating Tab Header (mini) screenshot](screenshots/floating-tab-header-mini.gif)
- **Hide Ribbon** ⭐
- **Hide Vault Title in Sidebar** ⭐ - hide the vault name in the left, makes sense if you only ever use one vault
- **Native Scrollbar styles** ⭐ - make scrollbars way nicer and color themed
- **Resize Handles** ⭐ - prefer more muted theme colours
- **Restrict Last Right Sidebar Panel** ⭐ - Sets max-height on last bottom right sidebar panel, saving you from constantly resizing the panel when resizing windows (e.g. for the calendar plugin panel, which is to me essential)
![Restrict last right sidebar panel screenshot](screenshots/restrict-last-right-sidebar-panel.png) 
- **Status bar tweaks** ⭐ - more visible text on dark theme 
- **Tab Header on bottom** - Move the tab title bar to the bottom, vertical statusbar when right sidedock closed
    ![Tab Header on Bottom screenshot](screenshots/tab-header-bottom.png)
- **Tab Header show path and title** ⭐ - I've disabled inline context filename editing and rely on this now, this shows the filename always without hover and allows rename with one click
- **Translucent Tab Header** - Classic style tab header showing blurred document content underneath (NOTE: its pretty, but on large documents causes performance issues delaying text due to the constant reflows caused by the graphical effect)
    ![Translucent Tab Header screenshot](screenshots/tab-header-translucent.png)
### User Snippets:
- **Daily Note styles** ⭐ - supporting styles for my daily note template, scoped to notes with `cssclass: dailynote` in frontmatter
- **Themed colours** ⭐ - Custom accent colours for each minimal theme subtheme, I like switchng minimal colour theme ocassionally and this ensures the accent color is overridden with a color that makes sense for the theme without needing to manually set it
    ![Themed Accents screenshot](screenshots/accents.gif)

### Plugin snippets
- **Calendar** ⭐ - Compact, weekend, day styles, colours, essential plugin for me
    ![Calendar screenshot](screenshots/calendar.png)
- **CardBoard** - Compact styles, waiting on feature update so WIP
    ![CardBoard screenshot](screenshots/cardboard.png)
 
- **Checklist (Ultra compact)** - Compact view (for tag mode users)    
    ![Checklist (ultra compact) screenshot](screenshots/checklist.png)
- **Custom Frames** ⭐ - Compact panel
- **Custom Frames (Duotone)** ⭐ - blend custom frames content in with theme until hover    
    ![Custom Frames - Duotone screenshot](screenshots/custom-frames-duotone.png)
- **Daily Note Outline** ⭐ - Compact, visual tweaks, works with compact file explorer snippet    
    ![Daily Note Outline screenshot](screenshots/daily-note-outline.png)
- **Database Folder (Compact)** - compact view    
    ![Database Folder screenshot](screenshots/dbfolder.png)
- **Make.MD Inline Context** ⭐ - Only used for banner functionality, inline context components are hidden. To use, add a `banner` property to a note's frontmatter directly or via Properties (see Autohide snippet)
    ![Make.MD Contexts screenshot](screenshots/makemdinlinecontexts.gif)
- **Make.MD Inline Context: Duotone Banner** ⭐- Makes all banner images duotone to match minimal theme    
    ![Make.MD Contexts Duotone banners screenshot](screenshots/makemdcontextsbannerduotone.png)
- **Make.MD Inline Context: Faded Banner** ⭐ Fade images to background with a gradient, and offsets text    
    ![Make.MD Contexts Gradient banners screenshot](screenshots/makemdcontextsbannergradient.png)
- **Meta Bind (Compact)** ⭐ - Inline controls are more compact, with customizations to some controls    
- **MySnippets** ⭐ - make menu wider and fix button style/order    
    ![MySnippets tweaks screenshot](screenshots/mysnippets_tweaks.png)
- **Omnisearch** ⭐ - Cleaner styles, less visual noise    
    ![Omnisearch screenshot](screenshots/omnisearch.png)
- **Outline** - chevron on right, compact    
    ![Outline tweaks screenshot](screenshots/outline.png)
- **Quiet Outline** - Remove rainbow colours to theme colors, re-arrange layout (I use this instead of Outline panel)
    ![Quiet Outline plugin tweaks screenshot](screenshots/quietoutline.png)
- **Smart 2nd Brain (compact)** - Some basic styles to fix some of the UX of this plugin, there are no class selectors in the plugin UI so its extremely hacky but makes it more compact  
    ![Smart second brain screenshot](screenshots/smart2ndbrain.png)
- **Tasks - Mono Icons (lucide2)** - Lucide2 Monotone icon set for Tasks Emoji Format, generated by [this tool I made](https://github.com/replete/obsidian-tasks-custom-icons)     
    ![Tasks - Mono Icons (lucide2) screenshot](screenshots/tasks-icons-lucide2.png)
- **Tasks - Compact** - Dates/backlink as tooltip. Colour-based priority. Incudes ['lucide2' monochrome tasks emojis](https://github.com/replete/obsidian-tasks-custom-icons).
    ![Tasks - Compact](screenshots/tasks-compact.gif)
- **Task progressbars** ⭐ - alignments and themed colours
    ![Task Progressbars plugin tweaks screenshot](screenshots/taskprogressbars.png)
- **Tracker** ⭐ - cleaner styles and duotone on hover
    
## Abandoned snippets (no longer developed)
- **Mono Emojis everywhere** - uses mono emoji font (activate separately) for everything in an editor (this is actually pretty ugly and I don't use it)  
- **Heatmap Calendar** - colours and text styles for habit type use-case [(imgur screenshot)](https://i.imgur.com/ndvRLIC.png)
- **Full Calendar** - pretty hacky due to limits of styling hooks
- **Obsidian Buttons** - alignments
- **Excel** - Follows minimal colour theme for plugin UI (excluding spreadsheet editor, which is a rendered canvas), tidy up some UI metrics
    ![Excel screenshot](screenshots/excel.png)
- **Day Planner** - ~~I'm using [my own fork](https://github.com/replete/obsidian-day-planner) of this abandoned plugin for more features but the styles here are not dependent on fork changes, yes its still buggy~~ Apparantly this plugin has a new maintainer, but I've stopped using it so these styles are for an older v
    ![Day Planner screenshot](screenshots/dayplanner.png)    


## Deprecated snippets (deleted from repo)
- ~~[Make.MD Banner](https://i.imgur.com/bn5bfMS.gif) - Mostly banner cssclass overrides, gradient, blur, tall, short etc - I refactored/improved this into separate snippets above~~
- ~~Make.MD Compact Spaces - use less space, like Compact File Explorer snippet (deprecated)~~
- ~~Make.MD Inline Context - Autohide meta ~~

## Support development
<a href="https://www.buymeacoffee.com/replete"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=replete&button_colour=BD5FFF&font_colour=ffffff&font_family=Poppins&outline_colour=000000&coffee_colour=FFDD00" /></a>

## TODO
- [x] Test/fix for Mobile Obsidian
- [x] Fix the weird list item alignments that vary depending on file length
- [x] Fix colour inconsistencies across light/dark themes
- [x] Test/fix for Windows (no fixes needed at time)
- [x] Test/fix for Linux (no fixes needed at time)

