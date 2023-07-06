# idealOS
How I wish my computers/devices worked.

### Content
<!-- MarkdownTOC levels="1,2,3" -->

- [Vision](#vision)
    + [General](#general)
    + [Specifics](#specifics)
- [Structure](#structure)
    + [Naming Conventions](#naming-conventions)
- [System](#system)
    + [Shell](#shell)
    + [Terminal](#terminal)
    + [Filesystem](#filesystem)
    + [Window Manager](#window-manager)
    + [File Manager](#file-manager)
    + [Editor/IDE](#editoride)
    + [Music Visualizer](#music-visualizer)

<!-- /MarkdownTOC -->

## Vision
### General
- Everything just works. Always. All the time.
- Open-source, free of control by for-profit entities.
- Learn from the mistakes of Windows, macOS, and Linux.
- Full user choice of hardware + software. No walled gardens.
- Beautiful, minimal UI. Consistent, delightful UX above all.
- Easy to use for normal people, fully hackable for hackers.
- Fast, seamless sync across every computer/device.
- Fast, automatic full system backup/restore.

### Specifics
- Core OS is tiny and lightning fast. No third-party bloat.
- Single desktop/mobile codebase. Optimized desktop/mobile UIs.
- Simple filesystem with well-defined structure.
- Text editing superpowers everywhere (modal/non-modal).
- Support legacy Windows, Linux, macOS, Android, iOS apps.

## Structure
```
/                            Root
├── .os                      OS directory (one place for *all* OS junk)
└── <user>                   User directory (one per user)
    ├── .cfg                 Single directory for all user apps and config
    │   ├── _src             System admin scripts
    │   ├── _env             System/environment settings (themes, fonts, package lists)
    │   └── <app>            App (one place for app and *all* its junk)
    │
    ├── arc                  The Archives
    │   ├── _arc             Archive of retired or inactive life pursuits
    │   ├── _lgx             Life logistics (car/house/medical/etc.)
    │   ├── cdx              The Codex - personal library (books/music/movies/etc)
    │   ├── navi             Public PKMS for notes taken during study of the Codex
    │   └── crow             Private PKMS for personal thoughts and other private info
    │       ├── _jnl         Life journals + topical journals
    │       └── <topic>      Active topic
    │
    ├── dev                  Engineering Projects
    │   ├── _arc             Archive of retired or inactive projects
    │   ├── _lgx             Logistics (scratch files, workspaces, etc.)
    │   └── <proj>           Active project
    │
    ├── lang                 Natural Language Learning Projects
    │   ├── _rosita          Language learning framework and progress tracking
    │   └── <xy>             ISO 639-1 two-letter language code
    │
    └── work                 A Necessary Evil
        ├── _admin           Resumes, credentials, job apps, etc.
        ├── _training        Institutional learning + other formal education/courses
        └── <job>            One directory per company/position
```

\_init.sh     Set up a new computer perfectly and effortlessly

### Naming Conventions
#### Prefixes
- `.` prefix - Hidden directories (to be sorted first and out of the way).
- `_` prefix - Meta-directories (to be sorted after hidden).
- no prefix - Standard data.

#### Patterns
- `_arc` - Archive. Convention for quarantining retired data.
- `_lgx` - Logistics. Convention for quarantining boring but necessary data.


## System
### Shell
### Terminal
### Filesystem

### Window Manager
- Titlebars
    * No icons
    * Center text
    * Change text/bg color based on active/inactive
    * Only show minimize/maximize/close buttons on hover
- Inspiration
    * https://www.reddit.com/r/unixporn/comments/zos11o/hyprland_mocha/


### File Manager
- oss, extendable, x-platform, fast
- move files between instances
- fuzzy finding and navigation
- compress/extract files/dirs
- file/image/video preview
- git status coloring
- configurable (theme, keymap, etc.)
- editor integration


### Editor/IDE
- **oss, extendable, x-platform, fast**
- Light enough to be an editor, powerful enough to be an IDE
- basic features
    + workspaces
    + sidebar (vcs-aware)
    + file tabs (vcs-aware)
    + statusline (vcs-aware)
    + regex find/repl (current file; open files/directories)
    + command palette
    + multiple cursors
    + snippets
    + minimap
- ui fully themable/schemable
- git integration
    + status/log/add/commit/push/pull
    + jump to next/prev change
    + revert change on line
    + preview change inline
    + add/commit hunks
    + minidiff gutter
- fuzzy-find symbols/files/everything
- jump to next/prev symbol
- inline colorcode highlighting
- LSP support
    + code completion
    + refactorring
    + jump to definition
    + hoverdocs
- DAP support
- nice config starter kits
- healthy PKMS package


### Music Visualizer
- https://youtu.be/wAZ6MnVueNY?t=65


### Disk Usage Analyzer
- `win` Ridnacs
