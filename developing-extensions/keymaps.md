# Keymaps

A command may have a corresponding keyboard shortcut. You can define key bindings for commands in keymap JSON files like below:

```javascript
{
  "ctrl-n": "application:new",
  "ctrl-c": "edit.copy",
  ...
}
```

Key binding should be a combination of following keys with `-` separator.

* **Character literals** : `a`, `1`, `,`, ...
* **Modifier keys** : `ctrl`, `cmd`, `shift`, `alt`, `cmdctrl` \(`cmdctrl` is automatically recognized in `cmd` in MacOS and `ctrl` in Windows and Linux and `alt` is corresponds to **option** key in MacOS\)
* **Special keys** : `enter`, `space`, `up`, `down`, `left`, `right`, `delete`, `tab`, `escape`, `backspace`, `home`, `end`, `pageup`, `pagedown`

The key bindings is shown in menu items of the same commands automatically.

The keymap JSON files should be placed in `keymaps/` folder of the extension and the keymap files are loaded in alphabetical order.

```text
my-extension/
└─ keymaps/
   └─ keymap.json
```

