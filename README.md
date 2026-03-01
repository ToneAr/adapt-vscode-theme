# Adapt VS Code

![logo](./images/icon.svg)

A complete adaptive theming solution for VS Code that automatically responds to your system accent color.

## What's Included

This extension pack bundles two extensions that work together to create a unified, accent-aware VS Code experience:

### 1. Adapt Theme (Color Theme)
A dynamic color theme that generates all UI colors based on your system accent color.

- Automatically detects your system accent color (KDE, GNOME, macOS, Windows)
- Generates a complete dark theme with colors derived from your accent
- Watches for system accent changes and updates in real-time
- Option to set a custom accent color

### 2. Adapt Icons (Icon Theme)
A dynamic icon theme that converts file and folder icons to monochrome using your accent color.

- Converts any icon set to monochrome with your accent color
- Supports loading icons from external icon theme sources
- Maintains icon shape/detail while unifying the color scheme
- Updates automatically when your accent color changes

## Features

- **Cross-Platform Support**: Works on Linux (KDE, GNOME), macOS, and Windows
- **Real-Time Updates**: Automatically detects and responds to system accent color changes
- **Unified Look**: Both theme and icons use the same accent color for a cohesive appearance
- **Customizable**: Override the system accent with any hex color you prefer
- **Lightweight**: Minimal performance impact

## Installation

1. Install this extension pack from the VS Code Marketplace
2. Open Command Palette (`Ctrl+Shift+P` / `Cmd+Shift+P`)
3. Select **Preferences: Color Theme** → **Adapt Dark**
4. Select **Preferences: File Icon Theme** → **Adapt Icons**

## Configuration

### Adapt Theme Settings

| Setting | Description | Default |
|---------|-------------|---------|
| `adaptTheme.accentColor` | Custom accent color (hex). Leave empty for system accent. | `""` |
| `adaptTheme.watchSystemAccent` | Auto-update when system accent changes | `true` |
| `adaptTheme.watchInterval` | Polling interval in milliseconds | `5000` |

### Adapt Icons Settings

| Setting | Description | Default |
|---------|-------------|---------|
| `adaptIcons.accentColor` | Custom accent color (hex). Leave empty for system accent. | `""` |
| `adaptIcons.iconThemeSourcePath` | Path to source icon theme for conversion | `""` |
| `adaptIcons.watchSystemAccent` | Auto-update when system accent changes | `true` |
| `adaptIcons.watchInterval` | Polling interval in milliseconds | `5000` |
| `adaptIcons.autoReload` | Auto-reload window on accent change | `false` |

## Commands

- **Adapt Theme: Refresh from System Accent** - Manually refresh the color theme
- **Adapt Theme: Set Custom Accent Color** - Set a custom accent color
- **Adapt Icons: Refresh from System Accent** - Manually refresh icons
- **Adapt Icons: Set Custom Accent Color** - Set a custom accent color for icons
- **Adapt Icons: Set Icon Theme Source Path** - Select an icon theme to convert
- **Adapt Icons: Debug Info** - Show debug information

## Using with External Icon Themes

The Adapt Icons extension can convert any compatible icon theme to monochrome:

1. Clone or download an icon theme (e.g., [A-WL File Icon Theme](https://github.com/ArturoWL/a-wl-file-icon-vscode))
2. Run command **Adapt Icons: Set Icon Theme Source Path**
3. Select the root folder of the icon theme
4. The icons will be converted to monochrome using your accent color

## Platform Support

| Platform | Accent Detection | Real-time Updates |
|----------|-----------------|-------------------|
| KDE Plasma | ✅ | ✅ (via dbus) |
| GNOME | ✅ | ✅ (via dconf) |
| macOS | ✅ | ✅ |
| Windows | ✅ | ✅ (via registry) |

## Screenshots

*Coming soon*

## Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

## License

MIT License - see [LICENSE](LICENSE) for details.
