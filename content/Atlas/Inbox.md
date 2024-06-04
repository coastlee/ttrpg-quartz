---
tag: map/view
---

up:: [[index|Home]]

# The Inbox
This isn't a normal inbox. It's a cooling pad 🧊.

Thoughts come in hot 🌶. But after a few days, they cool down ❄️.

When cooler thoughts prevail, you can better prioritize. Cool? 

This view looks at the 20 newest notes in your **+ Encounters** folder. As you process each note, make connections, add details, move them to the best folder,  and delete everything that no longer sparks ✨. 

> [!HINT]+ This data view 🔬 only renders in the free downloadable version.
> If you are viewing this note on Obsidian Publish, you won't be able to see the magic unless you [download the kit](https://www.linkingyourthinking.com/download-lyt-kit), but here's what it looks like in my personal vault... 
> ![[lyt-kit-example-cooling-pad-.jpg]] 
> If you can see the table below, you have already downloaded the LYT Kit.



``` dataview
TABLE WITHOUT ID
 file.link as Efforts,
 rank as "Rank"

FROM #effort

SORT rank desc




TABLE WITHOUT ID
 file.link as "Encounters and new notes",
 (date(today) - file.cday).day as "Days alive"

FROM "+ Encounters" and -#on/readme 

SORT file.cday asc

LIMIT 20
```
