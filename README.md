# flatpak_conf
configuration for apps inside sandboxes flatpak
---

### VSCodium
> i get problem with bash that is my default bash, i set default bash to fish then my vscodium/vscode cant load my fish into the app, so i found how to fix it
```
"terminal.integrated.profiles.linux": {
    "fish": {
        "path": "/app/bin/host-spawn",
        "args": ["fish"],
        "icon": "terminal-bash",
        "overrideName": true
    }
}
```
- paste this command into settings.json using shortcut `ctrl+shift+p` and type `settings.json` and then enter.
- so you can set default bash as you wamt but you need to restart the vscodium/vscode first.
- tips from me: i prefer to change the default bash using setting is not set using code instead because i can see if the bash was already.
- type this to search and replace the default bash into setting `terminal.integrated.defaultProfile`.
- use shortcut `ctrl+,(comma)` to open setting.
