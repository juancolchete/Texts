To make reload window shortcut works:

 1. Press `Ctrl + Shift + p` and open command pallet
 2. Type `keyboard shortcuts (JSON)` and press enter
 3. On the `keybindings.json` file:
 >- On the `key` field pass the shortcut
 >- On the `command` field pass workbench.action.reloadWindow
 >- On `when` field pass a empty string to this shortcut work without an specific condition
```
[
    {
        "key": "ctrl+f5",
        "command": "workbench.action.reloadWindow",
        "when": ""
    }
]
```