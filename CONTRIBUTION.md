# Contributing to Translucent Flyouts Config

Translucent Flyouts Config is a Free and Open-Source Software , and we welcome contributions from anyone who is interested in helping improve it. Whether you're a fellow developer, a translator, or a documentation writer, there are many ways to get involved.

## Background

Before you proceed I would like you to know that Translucent Flyouts Config was not meant for the public, but was a personal endeavour to make using Translucent Flyouts easier to use, for me. It was only when I approached the developer of Translucent Flyouts and it is because of his constant support, I am able to deliver a software that others can enjoy. I am really grateful for his help and efforts to make the FOSS community a better place.
Please show him some love and drop a ☆ star on his [repository](https://github.com/ALTaleX531/TranslucentFlyouts).

## Getting Started

If you are interested in contributing to Translucent Flyouts Config, you'll need to follow the underlying steps:

## Build and Run

Make sure you have Python v3.10.11 installed which works best with the current dependencies.

1. Clone the repository

```
git clone https://github.com/Satanarious/TranslucentFlyoutsConfig.git
```

2. Navigate to the project directory

```
cd TranslucentFlyoutsConfig
```

3. Install the required dependencies

```
pip install -r requirements.txt
```

4. Run

```
python main.py
```

## Directory Structure

```
🗀 TranslucentFlyoutsConfig
    🗀 Assets
        🗀 db
            - All JSONs holding program data
        🗀 fonts
            - Fonts for this application
        🗀 icons
            - Icons for this application
            🗀 dark
            🗀 light
    🗀 Data
        - Data fetched from JSONs
        - Static Information
        - Methods that return static information
    🗀 Generated
        - Files generated by pyuic6
    🗀 Global
        - Static methods that are called globally
    🗀 Readme
        - Readme translations
    🗀 Registry
        - Windows Registry management files
    🗀 Screenshots
        - Screenshots to attach in the Readme
    🗀 Scripts
        - .bat scripts to perform quick tasks
    🗀 Translations
        - All JSONs holding translation data
    🗀 UI_Files
        - .ui files created ui Qt Designer
    🗀 Widgets
        - Custom widgets created for this application
    main.py
    requirements.txt
```

## Contibution Guidelines

- The code should be well formatted and documented.
- I use [Ruff](https://docs.astral.sh/ruff/) for linting purpose, any warnings or errors regarding linting, can be because you using something else.
- Commits should be well-written and descriptive, with a clear summary of the changes made and any relevant context.
- Test all changes before creating a pull request and make sure they don't conflict with the exisiting features.
- Pull requests should target the `main` branch and include a clear summary of the changes made.

## Build Exe

To avoid any bugs, follow the underlying steps:

<details> <summary>Make sure <code>Assets/db/user_Settings.json</code> has the same values as <code>Assets/db/defaults.json</code></summary>

```
{
    "Global": {
      "Effect Type": 5,
      "Corner Type": 3,
      "Enable Drop Shadow": 0,
      "No Border Color": 0,
      "Enable Theme Colorization": 0,
      "Dark Mode Theme Colorization Type": 1,
      "Light Mode Theme Colorization Type": 1,
      "Dark Mode Border Color": "",
      "Light Mode Border Color": "",
      "Dark Mode Gradient Color": "",
      "Light Mode Gradient Color": "",
      "Enable Mini Dump": 1,
      "Disabled": 0,
      "Disabled List": [],
      "Block List": []
    },
    "DropDown": {
      "Effect Type": 9,
      "Corner Type": 4,
      "Enable Drop Shadow": 2,
      "No Border Color": 2,
      "Enable Theme Colorization": 2,
      "Enable Fluent Animation": 0,
      "Dark Mode Border Color": "",
      "Light Mode Border Color": "",
      "Dark Mode Gradient Color": "",
      "Light Mode Gradient Color": "",
      "Disabled": 2,
      "Disabled List": [],
      "Animation": {
        "Fade Out Time": 350,
        "Pop In Time": 250,
        "Fade In Time": 87,
        "Pop In Style": 0,
        "Start Ratio": 50,
        "Enable Immediate Interupting": 0
      }
    },
    "Menu": {
      "No System Drop Shadow": 0,
      "Enable Immersive Style": 1,
      "Enable Custom Rendering": 0,
      "Enable Fluent Animation": 0,
      "Enable Compatibility Mode": 0,
      "No Modern App Background Color": 1,
      "Color Treat As Transparent": "",
      "Color Treat As Transparent Threshold": 50,
      "Effect Type": 9,
      "Corner Type": 4,
      "Enable Drop Shadow": 2,
      "No Border Color": 2,
      "Enable Theme Colorization": 2,
      "Dark Mode Theme Colorization Type": 1,
      "Light Mode Theme Colorization Type": 1,
      "Dark Mode Border Color": "",
      "Light Mode Border Color": "",
      "Dark Mode Gradient Color": "",
      "Light Mode Gradient Color": "",
      "Disabled": 2,
      "Disabled List": [],
      "Animation": {
        "Fade Out Time": 350,
        "Pop In Time": 250,
        "Fade In Time": 87,
        "Pop In Style": 0,
        "Start Ratio": 50,
        "Enable Immediate Interupting": 0
      },
      "Disabled Hot": {
        "Corner Radius": 8,
        "Dark Mode Color": "",
        "Light Mode Color": "",
        "Enable Theme Colorization": 0,
        "Disabled": 0
      },
      "Focusing": {
        "Width": 1000,
        "Corner Radius": 8,
        "Dark Mode Color": "",
        "Light Mode Color": "",
        "Enable Theme Colorization": 0,
        "Disabled": 0
      },
      "Hot": {
        "Corner Radius": 8,
        "Dark Mode Color": "",
        "Light Mode Color": "",
        "Enable Theme Colorization": 0,
        "Disabled": 0
      },
      "Separator": {
        "Width": 1000,
        "Corner Radius": 8,
        "Dark Mode Color": "",
        "Light Mode Color": "",
        "Enable Theme Colorization": 0,
        "Disabled": 0
      }
    },
    "Tooltip": {
      "Effect Type": 9,
      "Corner Type": 4,
      "Enable Drop Shadow": 2,
      "No Border Color": 2,
      "Enable Theme Colorization": 2,
      "Margins Type": 0,
      "Margin Left": 6,
      "Margin Right": 6,
      "Margin Top": 6,
      "Margin Bottom": 6,
      "Dark Mode Color": "",
      "Light Mode Color": "",
      "Dark Mode Border Color": "",
      "Light Mode Border Color": "",
      "Dark Mode Gradient Color": "",
      "Light Mode Gradient Color": "",
      "Disabled": 2,
      "Disabled List": []
    }
  }
  

```

</details>

<details><summary> Make sure <code>Assets/db/app_settings.json</code> has the default values</summary>

```
{
  "Language": 0,
  "TFPath": "",
  "IconType": 0,
  "BackgroundColor": "#202020",
  "SecondaryBackgroundColor": "#313131",
  "LabelColor": "#FFFFFF",
  "TextColor": "#7A7A7A"
}
```

</details>

- Run the `Scripts/build_and_pack_for_release.bat` to build an executable which disabled the console window for the application or run `Scripts/build_and_pack_for_testing.bat` to build an executable with the console window enabled. You can modify these scripts to change the release version.

- This way you will get a `TranslucentFlyoutsConfigV{release_version}.zip` file in the project directory.

## Translation Contribution

You can contribute to the language of your choice that you are confident in contributing to for this project. You may wanna look at [this](Translations/hi-in.json) translation file before proceeding to contribute.

For first time contributors use the following Steps:

- Fork the Repository.
- Create a file in the [Translations directory](Translations/) using the name convention `LanguageCode-CountryCode.json`, all in lowercase.
- Copy everything from [hi-in.json](Translations/hi-in.json) and paste it into you new file.
- Remove Hindi translations for each corresponding English ones and replace with translation for your respective language.

> [!Important]
> There's a translations where a line ends with `<code>` and another that starts with `</code>`, pay close attention and keep it that way in you translation as well, else it will break the code.
> Here are the lines:
>
> - `"Uses the corresponding value in the global tab as the <code>"`
> - `"</code> value."`

If you wanna go a few steps further and edit python, you might as well follow these:

- Open [Data/enum.py](Data/enums.py) and add an additional value to the class ` Languages`.
- Open [Data/paths.py](Data/paths.py) and under class `Translations` add the path to you translation path in the exact way as mentioned there for the previously mentioned language(s).
- Open [Data/translations.py](Data/translations.py) and under class `TranslationModel`, under method `_fetch()`, find a dictionary `translationPath` and add another pair in the format `LanguageEnum:LanguageJSONPathVariable`
- Open [main.py](main.py) and under method `__init__` you will find a line which says `self.language` with a list of language names in their own languages. Add one for the one you are adding.

> [!Note]
> If you just wanna do the first part, I'll accept PR for the same as well and do the 2nd part myself. But the 2nd part would be appreciated.

## Bug Reports and Feature Requests

If you encounter a bug in Translucent Flyouts Config or have a feature request, please submit an issue. Please be sure to provide a clear description of the problem or feature request, along with any relevant context or steps to reproduce the issue.