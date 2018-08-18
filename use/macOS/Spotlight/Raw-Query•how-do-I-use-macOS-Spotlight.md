---
title: How do I use macOS Spotlight's Raw Data syntax?
---

# To enable
- Finder
- ⌘+⌥+[SPACE]
- "+" (next to Save)
- drop-down on "Name", choose "Other…"
- search "Raw query"
- enable checkbox
- "OK"

# To implement a Recently Created Smart Folder?
- Finder
- File | New Smart Folder
- "+" (next to Save)
- "Raw Query" from drop-down
- Enter (see below the process for obtaining this):
-- (kMDItemContentCreationDate = "*") && ((kMDItemContentTypeTree = public.content) || (kMDItemContentTypeTree = "com.microsoft.*"cdw) || (kMDItemContentTypeTree = public.archive))
- "Save" as "Recently Created"
- (optionally) File | Add to Sidebar, ^⌘T
## Skippable step: Obtaining the Raw Query String
- Open Recents in Finder
- Open Finde search, ⌘+⌥+[SPACE]
- "+" (next to Save)
- The RawQuery strign will be:
-- (kMDItemLastUsedDate = "*") && ((kMDItemContentTypeTree = public.content) || (kMDItemContentTypeTree = "com.microsoft.*"cdw) || (kMDItemContentTypeTree = public.archive))
- Replace the first term with kMDItemContentCreationDate


# SO article
- <https://apple.stackexchange.com/a/320729>

# Apple Developer docs
- <https://developer.apple.com/library/archive/documentation/Carbon/Conceptual/SpotlightQuery/Concepts/Introduction.html#//apple_ref/doc/uid/TP40001843-BBCFBCAG>
