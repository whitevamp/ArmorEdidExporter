```markdown
# Armor EDID Exporter

A Synthesis patcher script that exports the **Editor IDs (EDIDs)** of armors from selected Skyrim mods. It allows exporting the EDID list in either a **formatted style** or **plain text**, while filtering out armor items based on specific body part flags.

## Features

- **Export Armor EDIDs** in two formats:
  - **Formatted**: Outputs EDIDs in a structured format for further processing or scripting.
  - **Plain text**: Outputs a simple list of EDIDs.
- **Customizable Mod Selection**: Choose which mods you would like to include in the export.
- **Body Part Filtering**: Automatically excludes armor items that use the following body part flags:
  - Head
  - Hair
  - Circlet
  - Ring
  - Amulet

## Installation

1. Clone or download this repository.
2. Install [Synthesis](https://github.com/Mutagen-Modding/Synthesis) if you haven't already.
3. Add the `ArmorEdidExporter` script to your Synthesis patcher.

## Usage

1. Run the Synthesis patcher.
2. Configure the patcher settings:
   - **Formatted EDID**: Toggle to export the EDID list in a formatted style.
   - **Plain text EDID**: Toggle to export the EDID list as plain text.
   - **Mods to Include**: Select the mods from which you want to export armor EDIDs.
3. The script will export the armor EDID list to two separate files based on the selected format(s):
   - `FormattedArmorEDID.txt`
   - `PlainArmorEDID.txt`

## Settings

In the Synthesis patcher, you will find the following customizable settings:

- **Formatted EDID**: Export the armor EDID list in a formatted style.
- **Plain text EDID**: Export the armor EDID list in plain text.
- **Mods to Include**: Select which mods to include in the export. If no mods are selected, all available mods will be processed.

### Example of Formatted EDID Output

```
if (Settings.kwdSettings.Blank && (StrMatch(name, "Armor1")))
if (Settings.kwdSettings.Blank && (StrMatch(name, "Armor2")))
if (Settings.kwdSettings.Blank && (StrMatch(name, "Armor3")))
```

### Example of Plain Text EDID Output

```
Armor1
Armor2
Armor3
```

## Requirements

- [Skyrim Special Edition](https://store.steampowered.com/app/489830/The_Elder_Scrolls_V_Skyrim_Special_Edition/)
- [Synthesis](https://github.com/Mutagen-Modding/Synthesis)

## How to Contribute

Contributions, issues, and feature requests are welcome! Feel free to check out the [issues page](https://github.com/yourusername/ArmorEdidExporter/issues).

1. Fork the repository.
2. Create your feature branch (`git checkout -b feature/NewFeature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the branch (`git push origin feature/NewFeature`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

- Developed using the [Mutagen](https://github.com/Mutagen-Modding/Mutagen) library.
- Patcher powered by [Synthesis](https://github.com/Mutagen-Modding/Synthesis).

```
