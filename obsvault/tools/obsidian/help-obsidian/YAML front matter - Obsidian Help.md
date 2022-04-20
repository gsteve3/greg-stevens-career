---
created: 2022-04-18T12:14:58 (UTC -06:00)
tags: []
source: https://publish.obsidian.md/
author: 
---
# YAML front matter - Obsidian Help

> # YAML front matter - Obsidian Help
> YAML, also known as front matter, is designed to be file-level metadata that is readable by humans _and_ Obsidian.
> 
> Front matter is a section of plain text attributes that starts at the first line of the file. It is one of the most popular ways to add metadata in a Markdown file, and has been popularized by static generators such as Jekyll, Hugo, and Gatsby.
> 
> A YAML block needs **triple dashes** at the start and end to be read by Obsidian (and other apps). It also needs to be placed at the very top of the file.
> 
> For example:
> 
> ```
> ---
> key: value
> key2: value2
> key3: [one, two, three]
> key4:
> - four
> - five
> - six
> ---
> ```
> 
> As of 0.12.12, there are four keys natively supported:
> 
> -   `tags` ([more information](https://help.obsidian.md/How+to/Working+with+tags))
> -   `aliases` ([more information](https://help.obsidian.md/How+to/Add+aliases+to+note))
> -   `cssclass`
> -   `publish` ([Publish and unpublish notes > Automatically select notes to publish](https://help.obsidian.md/Obsidian+Publish/Publish+and+unpublish+notes#Automatically%20select%20notes%20to%20publish) and [Publish and unpublish notes > Ignore notes](https://help.obsidian.md/Obsidian+Publish/Publish+and+unpublish+notes#Ignore%20notes))
> 
> As Obsidian continues to develop, we will gradually make it more accessible by plugin developers, and make it more user friendly.
> 