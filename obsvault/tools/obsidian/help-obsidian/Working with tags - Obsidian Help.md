---
original_title: Working with tags - Obsidian Help
source: https://publish.obsidian.md/
clip_date: 2022-04-20T13:55:24 (UTC -06:00)
tags:
  - WebClip
excerpt: YAML front matter
---


---
Tags are a very useful way of grouping multiple notes so they are easy to find. A tag is essentially a clickable search through your entire Vault for a term. For example, clicking on [#tags](https://publish.obsidian.md/#tags) will bring up a search with all notes that contain that tag. Most people use them for broad categories of things, like a class you might be taking notes in or a type of idea. Some Zettelkasten practitioners like to use them as "entry points" for thinking about connected ideas. But ultimately, they are flexible enough that you can use them in any way you would like.

### Add tags

Just type `#` followed by tag name like `#tag1`  
You can also add tags in the notes [YAML front matter](https://help.obsidian.md/Advanced+topics/YAML+front+matter) like so:

```
---
tags:
  - tag1
  - tag2
---
```

### Tag pane

If you have the [Tag pane](https://help.obsidian.md/Plugins/Tag+pane) plugin enabled, you will see a list of all tags that are used across all of your notes, sorted by frequency. Clicking on any of those will activate that search.

This will allow you to search exact matches of a tag. For example, when clicking , as per usual, but if you want to find all instances of `maintag` with all subtags, you can still use the [Search](https://help.obsidian.md/Plugins/Search) to look for `#maintag`. This is useful in cases where you have subcategories of things but you also want to be able to easily find all instances of the higher category.

### Allowed characters

Spaces are not allowed in tags. So, to differentiate two or more words in a tag, you can use these case styles/formats:

-   camelCase: [#twoWords](https://publish.obsidian.md/#twoWords)
-   PascalCase: [#TwoWords](https://publish.obsidian.md/#TwoWords)
-   snake\_case: [#two\_words](https://publish.obsidian.md/#two_words)
-   kebab-case: [#two-words](https://publish.obsidian.md/#two-words)

The only symbols allowed are:

1.  `_` (underscore) and `-` (dash) to separate words;
2.  `/` (forward slash) for [nested tags](https://help.obsidian.md/Plugins/Tag+pane#Nested%20tags).

Numbers are allowed in the tag, as long as the tag is not purely numeric. For example, #1984 isn't a valid tag, but [#y1984](https://publish.obsidian.md/#y1984) is a valid one.
