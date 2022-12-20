# idealOS
How I wish my computers/devices worked.

### Content
<!-- MarkdownTOC -->

- [Vision](#vision)
    + [General](#general)
    + [Specifics](#specifics)
- [FS Structure](#fs-structure)
    + [Naming Conventions](#naming-conventions)
- [Apps](#apps)
    + [Window Manager](#window-manager)
    + [Editor/IDE](#editoride)

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

## FS Structure
```
/
├── .os                         Single directory for *all* OS junk
└── <user>                      Single directory for each user
    ├── .config                 Single directory for all user apps and configuration
    │   ├── _admin
    │   │   └── _bootstrap.sh   Set up a new computer with all apps and data configured perfectly
    │   ├── _apps
    │   │   └── <app>           Single directory for each app and *all* its junk
    │   └── _env                System/environment settings and stuff (themes, fonts, package lists)
    │
    ├── archives                Second brain/notes and reference data that mostly just sits there
    │   ├── _logistics          Life logistics I don't care too much about (house/car/finances)
    │   ├── _media              Books/music/movies/shows
    │   └── jiki                Interesting things I actually care about
    │       ├── _journals       Life journal + topic-focused journals
    │       └── <thing>
    │
    ├── dev                     Software projects
    │   ├── _archived           Convention to get retired projects out of sight
    │   └── <project>
    │
    ├── langs                   Language-learning projects
    │
    └── work                    A necessary evil
        ├── _admin              Resumes, credentials, job apps, etc.
        ├── _training           Institutional learning + other formal education/courses
        └── <job>
```

### Naming Conventions
- `.` prefix - For hidden directories, to be sorted first and out of the way.
- `_` prefix - For meta-directories, to be sorted after hidden.
- no prefix - For all standard content.


## Apps
### Window Manager
- Titlebars:
    * No icons
    * Center text
    * Change text/bg color based on active/inactive
    * Only show minimize/maximize/close buttons on hover


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
- ui
    + minimap
    + themable/schemable
    + git-aware project tree/tabs/statusline
- multiple cursors
- git integration
    + status/log/add/commit/push/pull
    + jump to next/prev change
    + revert change on line
    + add/commit hunks
    + minidiff gutter
- regex find/repl (current file; open files/directories)
- workspaces
- snippets
- fuzzy-find symbols/files/everything
- jump to next/prev symbol
- inline colorcode highlighting
- LSP support
    + code completion
    + refactorring
    + jump to definition
    + hoverdocs
- DAP support
- command palette
- nice config starter kits
- healthy PKMS package
