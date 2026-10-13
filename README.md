# macOS Modern — Mailspring Theme

A refined, native Apple Mail light theme for [Mailspring](https://getmailspring.com) built with modern typography, frosted sidebars, capsule search bars, and clean macOS aesthetics.

---

## ✨ Features

- **Native Apple Typography**: Seamless integration with Apple's `-apple-system` and SF Pro typography hierarchy.
- **Frosted Sidebar**: Subtle gray sidebar (`#F2F2F7`) with rounded selection pills and Apple-style badge counters.
- **Modern macOS Toolbar & Capsule Search**: Smooth search field with focus glow and streamlined action buttons.
- **Polished Thread List**: Crisp row spacing, Apple system blue unread indicators, and native macOS list selection highlights.
- **Card-Based Reading Pane**: Clean reading view with subtle border separation, modern contact pills, and attachment badges.
- **Apple Blue Composer**: Distraction-free composing experience with rounded inputs and native Apple blue action buttons.
- **Modular LESS Architecture**: Cleanly separated into modular `.less` stylesheets for effortless customization.

---

## 🚀 Installation

### Option 1: Symlink for Live Development (Recommended)

Link this repository directly to your Mailspring packages directory so that changes reflect immediately:

```bash
# macOS
ln -s "/Users/colbydolly/Documents/Mailspring theme" ~/Library/Application\ Support/Mailspring/packages/mailspring-macos-modern
```

Then open **Mailspring** and select:
> **Preferences (`Cmd + ,`) > Appearance > Choose "macOS Modern"**

### Option 2: Install via Mailspring UI

1. Open **Mailspring**.
2. Go to the menu bar: **Mailspring > Install New Theme...**
3. Select this repository folder (`Mailspring theme`).
4. Activate the theme in **Preferences > Appearance**.

---

## 🛠 Live Development & Reloading

To quickly test changes without restarting Mailspring:

1. In Mailspring, navigate to **Developer > Toggle Developer Tools** (or press `Cmd + Option + I`).
2. In the Developer Console, reload the theme instantly:
   ```javascript
   AppEnv.themes.setActiveTheme('ui-light');
   AppEnv.themes.setActiveTheme('mailspring-macos-modern');
   ```

---

## 🎨 Customizing Theme Colors

All primary design tokens and colors are located in `styles/ui-variables.less`. You can easily tweak:

- **Accent Color**: Modify `@apple-blue` (default: `#007aff`) to your preferred accent (e.g. purple `#af52de`, orange `#ff9500`, or teal `#30b0c7`).
- **Sidebar Background**: Adjust `@sidebar-background` (default: `#f2f2f7`).
- **Font Stack**: Update `@font-family` to use custom fonts.

---

## 📂 Project Structure

```text
mailspring-macos-modern/
├── package.json               # Theme metadata & Mailspring configuration
├── README.md                  # Theme documentation & usage
├── LICENSE                    # MIT License
├── .gitignore                 # Git ignore rules
└── styles/
    ├── index.less             # Main stylesheet entry point
    ├── ui-variables.less      # Design tokens and color variables
    ├── theme-colors.less      # Theme picker swatch preview
    ├── sidebar.less           # Navigation sidebar styling
    ├── toolbar.less           # Titlebar toolbar and capsule search
    ├── threadlist.less        # Email thread list view
    ├── messagelist.less       # Email message reading pane
    ├── composer.less          # Email composer modal and inputs
    ├── window-controls.less   # macOS traffic light controls
    └── components.less        # Menus, dropdowns, and overlay scrollbars
```

---

## 📄 License

This theme is open-source and licensed under the [MIT License](LICENSE).
