## [Windows Terminal](https://github.com/Microsoft/Terminal)

### Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

```
    git clone https://github.com/thanos-theme/windows-terminal.git
```

### Install manually

Download using the [GitHub .zip download](https://github.com/thanos-theme/windows-terminal/archive/master.zip) option and unzip them.

### Install using windows-terminal `settings.json`

1.  Start Windows Terminal and press `ctrl+,` to open the settings
2.  Now click on the option: `Open JSON file` on the bottom-left corner of the screen
3.  Inside of `settings.json` file find the `"schemes":` key and paste the contents of the version you chose inside of `/themes/dark` or `/themes/light`.

    Example:

    ```
    [...]

    "schemes":[

        {
            "name": "Thanos - Infinity Dark",
            "cursorColor": "#C4C5B5",
            "selectionBackground": "#2A3049",
            "background": "#181B28",
            "foreground": "#C4C5B5",
            "black": "#1A1A1A",
            "blue": "#9d65ff",
            "cyan": "#9d65ff",
            "green": "#58ebd7",
            "purple": "#00A1E4",
            "red": "#ff206e",
            "white": "#C4C5B5",
            "yellow": "#FABC2A",
            "brightBlack": "#625E4C",
            "brightBlue": "#9d65ff",
            "brightCyan": "#9d65ff",
            "brightGreen": "#58ebd7",
            "brightPurple": "#00A1E4",
            "brightRed": "#ff206e",
            "brightWhite": "#F6F6EF",
            "brightYellow": "#FABC2A"
        }
    ]

    [...]
    ```

4.  Remember to save your `settings.json` file. You may need to give permission to your editor to do that.

### Activating theme

> You can activate the theme either through the `settings.json` file you're currently at or through the `settings UI` that was opened when you pressed `ctrl+,`

#### Activation through `settings.json`

1. To activate your theme through the `settings.json` file you just need to find the `"profiles":` key and change the `colorScheme` property to the `name` of the theme you just added.
   Example:

   ```
   [...]

   "profiles":{
       "defaults":{
           "colorScheme":"Thanos - Infinity Dark"
       }
   }

   [...]
   ```

2. If you prefer to change it for a specific profile you should change the `colorScheme` inside of `list`.
   Example:

   ```
   [...]

   "profiles":{
       "defaults":{},
       "list":[
           {
               "name":"Ubuntu",
               "colorScheme":"Thanos - Infinity Dark"
           },
           // other profiles
       ]
   }

   [...]
   ```

#### Activation through `settings UI`

1. To activate your theme through the `settings UI` you should navigate to the tab `Color Schemes` and choose the theme variant you selected on the dropdown menu.
2. If you want to set the theme for a specific profile, you should navigate to that profile under the `Profiles` section and navigate to the `Appearance` tab under `Additional Settings`.
3. Then you can change the theme under the option `Color scheme`
