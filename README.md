# cs2-custom-menu
**a plugin to create customizable menus**
> supports chat, centerhtml & wasd menu
>
> permission based or team based menus and commands
>
> every menu and menu option has a bunch of settings, <a href="#config-example">see examples</a>

<br>

<details>
	<summary>showcase</summary>
	<video src="https://github.com/user-attachments/assets/07574910-1b56-48e4-90de-39342743bdaa">
</details>

<br>

## information:

### requirements
- [MetaMod](https://github.com/alliedmodders/metamod-source)
- [CounterStrikeSharp](https://github.com/roflmuffin/CounterStrikeSharp)
- [Interesting-exe/WASDMenuAPI](https://github.com/Interesting-exe/WASDMenuAPI) (optional)
- [T3Marius/CS2ScreenMenuAPI](https://github.com/T3Marius/CS2ScreenMenuAPI) (optional)
<br>

## example config
<a name="config-example"></a>
**Messages** - Default: `true` (sends no permission & selecting message) <br>

**Title** - Default: `"Menu"` (title of the menu) <br>
**Type** - Default: `"html"` (options: chat/html/wasd/screen) <br>
**Command** - Defualt: `""` (you can use multiple by splitting them with `,`) <br>
**Permission** - Default: `""` (empty for no check, @css/reservation for vip) <br>
**Team** - Default: `""` (T for Terrorist, CT for CounterTerrorist or empty for both) <br>

**Sound** - Default: `""` (use vsnd like sounds/buttons/blip1.vsnd) <br>
**CloseMenu** - Default: `false` (close the menu on select) <br>
**Confirm** - Default: `false` (opens a confirmation menu on select) <br>
**Cooldown** - Default: `0` (how many seconds until the command can be used again) <br>

```json
{
  "Prefix": "{green}[Menu]{default}",
  "Messages": true,
  "Menus": {
    "1": {
      "Title": "Example Menu",
      "Type": "html",
      "Command": "css_examplemenu",
      "Permission": "",
      "Team": "",
      "Options": [
        {
          "Title": "Example Option",
          "Command": "",
          "Permission": "",
          "Team": "",
          "Sound": "",
          "CloseMenu": false,
          "Confirm": false,
          "Cooldown": 0
        },
        {
          "Title": "Example Option 2",
          "Command": "css_example2",
          "Permission": "@css/root",
          "Team": "T",
          "Sound": "sounds/buttons/blip1.vsnd",
          "CloseMenu": true,
          "Confirm": true,
          "Cooldown": 3
        }
      ]
    }
  }
}
```

<br> <a href="https://ko-fi.com/exkludera" target="blank"><img src="https://cdn.ko-fi.com/cdn/kofi5.png" height="48px" alt="Buy Me a Coffee at ko-fi.com"></a>
