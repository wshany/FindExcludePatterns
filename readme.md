**[Sublime Text 3+](http://www.sublimetext.com/) Package**. Install via an updated version of  [Package Control](https://sublime.wbond.net/installation). Just **DON'T** install manually.

# Find Exclude Patterns

## Description

"Find in Files" command includes a lot of noise from binary files, folders you don't want to include in search (caches, generated files, logs, version control, external libraries, etc, etc, etc). The current way to exclude these from searches... is to manually select the list for every search... ! insane.

When installed, this package will automatically append negative values ("please don't search XYZ") to the "where" parameter every time you open the the "Find in Files" panel.

## Preferences

By default will exclude the following normal Sublime Text preferences: "index_exclude_patterns" and "binary_file_patterns". Plus a new preference named "find_exclude_patterns". These preferences default to an empty list or array when blank or not used.

To edit your preferences just go to: Main menubar -> Preferences -> Settings - User.

TIP: To exclude a folder you need to write it like this: "\*/.git/\*". Then for example to exclude version control from searches your preference will looks somewhat like this:

    "find_exclude_patterns": ["*/.svn/*", "*/.git/*", "*/.hg/*", "*/CVS/*"]

## Source-code

https://github.com/titoBouzout/FindExcludePatterns

## Forum Thread

http://www.sublimetext.com/forum/viewtopic.php?f=5&t=18978
