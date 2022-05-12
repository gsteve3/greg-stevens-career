---
created: 2022-05-12T08:46:46-06:00
updated: 2022-05-12T09:11:52-06:00
---

https://help.obsidian.md/Advanced+topics/Using+obsidian+URI

```
obsidian://open?vault=my%20vault&file=my%20note.md
```


obsidian://open?vault=obsvault&file=

---


## Config
### Tweaked

`/.vscode/settings.json:1`
```jsonc
{
    "files.eol": "\n",
    "files.insertFinalNewline": false,
    "conventionalCommits.scopes": [
        "obsidian",
        "ui"
    ],
    "open.fileMappings": [

        {
            "output2": "obsidian://open?vault=obsvault&file=../${editor:relativeFile}",
            "pattern2": "${editor:file}",
            "pattern": "(?<group_1>obsvault\\\\)(?<group_2>(.+?)*)",
            "output": "obsidian://open?vault=obsvault&file=${match:group_2}",
            "lineSeparator": "#",
            "linePrefix": "L"
        }
    ],
    "open.prMappings": [
        {
            "pattern": "${editor:file}",
            "provider": {
                "type": "phabricator",
                "base": "https://phabricator.example.com"
            }
        }
    ],
    "open.uriMappings": [
        {
            "pattern": "https://host.example.com/repo/${regex:file}${regex:lines}",
            "output": "${editor:workspaceFolder}/${match:file}${match:lines}",
            "lineSeparator": "#"
        }
    ]
}

```


### Original from GitHub

https://github.com/alexander-yu/vscode-open


{
    "open.fileMappings": [
        {

            "pattern": "src/static/(?<mdFileWithoutExt>.+)\\.md$",
            "output": "https://host.example.com/docs/${match:mdFileWithoutExt}"
        },
        {
            "pattern": "${editor:file}",
            "output": "https://host.example.com/repo/${editor:relativeFile}${editor:lines}",
            "lineSeparator": "#",
            "linePrefix": "L"
        }
    ],
    "open.prMappings": [
        {
            "pattern": "${editor:file}",
            "provider": {
                "type": "phabricator",
                "base": "https://phabricator.example.com"
            }
        }
    ],
    "open.uriMappings": [
        {
            "pattern": "https://host.example.com/repo/${regex:file}${regex:lines}",
            "output": "${editor:workspaceFolder}/${match:file}${match:lines}",
            "lineSeparator": "#"
        }
    ]
}


{
    "open.fileMappings": [
        {

            "pattern": "(?<mdFileWithoutExt>.+)\\.md$",
            "output": "obsidian://open?vault=obsvault&file=${match:mdFileWithoutExt}"
        },
        {
            "pattern": "${editor:file}",
            "output": "https://host.example.com/repo/${editor:relativeFile},
            "lineSeparator": "#",
            "linePrefix": "L"
        }
    ],
    "open.prMappings": [
        {
            "pattern": "${editor:file}",
            "provider": {
                "type": "phabricator",
                "base": "https://phabricator.example.com"
            }
        }
    ],
    "open.uriMappings": [
        {
            "pattern": "https://host.example.com/repo/${regex:file}${regex:lines}",
            "output": "${editor:workspaceFolder}/${match:file}${match:lines}",
            "lineSeparator": "#"
        }
    ]
}

