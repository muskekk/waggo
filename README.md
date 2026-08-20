[site](https://muskekk.github.io/waggo)

# Waggo — Code Be Freely

Waggo is a lightweight, browser-based code editor inspired by Kate and built with the Monaco Editor.

It provides syntax highlighting, multiple files, HTML preview, themes, keyboard shortcuts, a command palette, and local file operations — all inside a single HTML file.

---

## Features

- Monaco Editor integration
- Syntax highlighting
- Multiple open documents
- HTML live preview
- Run HTML directly in the browser
- Open local files
- Download/save the current file
- Command Palette
- Custom keyboard shortcuts
- Dark, Light, and High Contrast themes
- Adjustable editor font size
- Sidebar for open documents
- Persistent settings and tabs when browser storage is available
- Automatic operating system detection
- Responsive browser-based interface
- No build system required

---

## Requirements

Waggo runs directly in a modern web browser.

Recommended browsers:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox
- Safari

An internet connection is recommended because Waggo loads Monaco Editor and Google Fonts from external CDNs.

---

## Installation

No installation or build process is required.

### 1. Save the file

Save the provided HTML code as:

```text
waggo.html
```

### 2. Open it

Double-click `waggo.html` or open it with your browser.

For example:

```text
File → Open File → waggo.html
```

Waggo will display a short startup screen and then open the editor.

---

## Basic Usage

### Creating a new file

Click:

```text
File → New File
```

or click the `＋` button in the sidebar.

The default language for a new file is HTML.

Default shortcut:

```text
Ctrl + Alt + N
```

On macOS:

```text
⌘ + ⌥ + N
```

---

## Editing Code

The main area is the Monaco Editor.

You can write and edit code just like in VS Code.

For example:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Hello Waggo</title>
</head>
<body>
    <h1>Hello, Waggo!</h1>
</body>
</html>
```

Waggo automatically provides syntax highlighting based on the selected language.

---

## Selecting a Programming Language

Use the language selector in the toolbar.

Supported languages include:

- HTML
- CSS
- JavaScript
- TypeScript
- JSON
- Python
- Java
- C
- C++
- C#
- Go
- Rust
- PHP
- Ruby
- Markdown
- YAML
- XML
- SQL
- Shell
- Plain Text

Example:

```text
HTML
CSS
JavaScript
Python
Rust
```

When you change the language, Waggo also updates the file extension.

For example:

```text
untitled1.html
```

can become:

```text
untitled1.py
```

when Python is selected.

---

# Running HTML

Waggo can execute HTML directly inside the browser.

Create an HTML file and write your code:

```html
<!DOCTYPE html>
<html>
<body>

<h1>Hello World!</h1>

<button onclick="alert('Hello from Waggo!')">
    Click Me
</button>

</body>
</html>
```

Then click:

```text
▶ Run
```

The preview panel will open automatically.

You can also use:

```text
View → Toggle Preview
```

or the keyboard shortcut:

```text
Ctrl + Alt + P
```

On macOS:

```text
⌘ + ⌥ + P
```

---

# Preview Panel

The Preview panel appears on the right side of the editor.

It contains:

- Refresh button
- Close button
- HTML output

The preview is rendered inside a sandboxed iframe.

You can refresh the preview with:

```text
⟳
```

To close it:

```text
✕
```

---

# Opening Local Files

To open an existing file:

```text
File → Open…
```

Waggo will open the browser's file picker.

You can select files such as:

```text
index.html
style.css
script.js
app.py
main.cpp
README.md
```

Waggo determines the language from the file extension.

---

# Saving a File

Waggo does not use a traditional server-side save system.

Instead, use:

```text
File → Save As…
```

or:

```text
Ctrl + Alt + S
```

On macOS:

```text
⌘ + ⌥ + S
```

The current document is downloaded to your computer.

For example:

```text
index.html
```

will be downloaded as an HTML file.

---

# Multiple Documents

Waggo supports multiple open documents.

All open documents are shown in the left sidebar.

Example:

```text
Open Documents

● index.html
● style.css
● script.js
● README.md
```

Click a document to switch to it.

Click:

```text
✕
```

to close a document.

---

# Sidebar

The sidebar contains all currently open documents.

Toggle it using:

```text
View → Toggle Sidebar
```

or:

```text
Ctrl + Alt + B
```

On macOS:

```text
⌘ + ⌥ + B
```

You can also use the:

```text
▤ Sidebar
```

button in the toolbar.

---

# Command Palette

The Command Palette allows you to quickly search for commands, languages, themes, and open files.

Open it with:

```text
Alt + Space
```

You can also click:

```text
Search commands, files, settings…
```

Example searches:

```text
new file
preview
theme
python
javascript
sidebar
zoom
settings
```

The search uses fuzzy matching, so you do not need to type the exact command name.

---

# Themes

Waggo includes three themes.

## Waggo Dark

The default dark theme.

```text
Waggo Dark
```

## Waggo Light

A light editor theme.

```text
Waggo Light
```

## Waggo Contrast

A high-contrast black and yellow theme.

```text
Waggo Contrast
```

You can change the theme using the toolbar:

```text
Theme → Waggo Dark
```

or:

```text
Settings → Preferences…
```

You can also cycle through themes with:

```text
Ctrl + Alt + T
```

On macOS:

```text
⌘ + ⌥ + T
```

---

# Changing Editor Font Size

Use:

```text
View → Zoom In
```

or:

```text
Ctrl + Alt + =
```

To zoom out:

```text
View → Zoom Out
```

or:

```text
Ctrl + Alt + -
```

The font size is limited between 9px and 32px.

---

# Keyboard Shortcuts

The default shortcuts are:

| Command | Windows / Linux | macOS |
|---|---|---|
| Command Search | Alt + Space | Alt + Space |
| New File | Ctrl + Alt + N | ⌘ + ⌥ + N |
| Close Tab | Ctrl + Alt + W | ⌘ + ⌥ + W |
| Save As | Ctrl + Alt + S | ⌘ + ⌥ + S |
| Run HTML | Ctrl + Alt + Enter | ⌘ + ⌥ + Enter |
| Toggle Preview | Ctrl + Alt + P | ⌘ + ⌥ + P |
| Toggle Sidebar | Ctrl + Alt + B | ⌘ + ⌥ + B |
| Next Tab | Ctrl + Alt + ] | ⌘ + ⌥ + ] |
| Previous Tab | Ctrl + Alt + [ | ⌘ + ⌥ + [ |
| Preferences | Ctrl + Alt + , | ⌘ + ⌥ + , |
| Keyboard Shortcuts | Ctrl + Alt + K | ⌘ + ⌥ + K |
| Cycle Theme | Ctrl + Alt + T | ⌘ + ⌥ + T |
| Zoom In | Ctrl + Alt + = | ⌘ + ⌥ + = |
| Zoom Out | Ctrl + Alt + - | ⌘ + ⌥ + - |

Waggo automatically detects whether you are using Windows, Linux, or macOS.

---

# Custom Keyboard Shortcuts

Every Waggo command can be remapped.

Open:

```text
Settings → Keyboard Shortcuts…
```

or use:

```text
Ctrl + Alt + K
```

On macOS:

```text
⌘ + ⌥ + K
```

You will see a list of commands and their current shortcuts.

For example:

```text
New File                  Ctrl + Alt + N
Close Current Tab        Ctrl + Alt + W
Save As                   Ctrl + Alt + S
Run HTML                  Ctrl + Alt + Enter
Toggle Preview            Ctrl + Alt + P
```

Click:

```text
Change
```

Then press the desired key combination.

Press:

```text
Esc
```

to cancel recording.

---

# Shortcut Conflicts

Waggo prevents two Waggo commands from using the same shortcut.

If you assign a shortcut that is already assigned to another Waggo command, the old command's shortcut will be removed.

For example:

```text
New File → Ctrl + Shift + N
```

If another command already uses:

```text
Ctrl + Shift + N
```

that command will lose its shortcut.

You can restore all shortcuts using:

```text
Reset all to defaults
```

---

# Browser Shortcuts

Waggo intentionally avoids overriding important browser shortcuts.

For example, browser shortcuts such as:

```text
Ctrl + T
Ctrl + W
Ctrl + Tab
Ctrl + Shift + T
```

are not used as Waggo's default shortcuts.

This helps prevent conflicts with Chrome, Firefox, Edge, and other browsers.

---

# Settings

Open Settings using the gear button:

```text
⚙
```

or:

```text
Settings → Preferences…
```

The Settings window contains three sections.

## General

Contains:

- Theme selection
- Operating system information
- General Waggo information

## Keyboard Shortcuts

Contains:

- All Waggo commands
- Current shortcuts
- Change buttons
- Reset buttons
- Reset all shortcuts

## About

Displays information about Waggo.

Current version:

```text
0.1.0
```

---

# Session Persistence

Waggo attempts to remember your:

- Open documents
- Document contents
- Active document
- Theme
- Sidebar state
- Preview state
- Editor font size
- Keyboard shortcuts

This uses the available browser storage API.

If persistent storage is unavailable, Waggo still works as a normal browser-based editor, but settings may not survive a reload.

---

# File Extensions

Waggo maps common extensions to Monaco languages.

| Extension | Language |
|---|---|
| `.html` | HTML |
| `.css` | CSS |
| `.js` | JavaScript |
| `.ts` | TypeScript |
| `.json` | JSON |
| `.py` | Python |
| `.java` | Java |
| `.c` | C |
| `.cpp` | C++ |
| `.cs` | C# |
| `.go` | Go |
| `.rs` | Rust |
| `.php` | PHP |
| `.rb` | Ruby |
| `.md` | Markdown |
| `.yml` | YAML |
| `.xml` | XML |
| `.sql` | SQL |
| `.sh` | Shell |
| `.txt` | Plain Text |

---

# Example Workflow

A typical workflow looks like this:

### 1. Open Waggo

```text
waggo.html
```

### 2. Create a new HTML file

```text
File → New File
```

### 3. Write HTML

```html
<!DOCTYPE html>
<html>
<head>
    <title>My Page</title>
</head>
<body>
    <h1>Hello Waggo!</h1>
</body>
</html>
```

### 4. Run it

Click:

```text
▶ Run
```

### 5. Check the preview

The page will appear in the Preview panel.

### 6. Save the file

Use:

```text
File → Save As…
```

and save it as:

```text
index.html
```

---

# Architecture

Waggo is implemented as a single HTML document.

The main technologies are:

- HTML
- CSS
- JavaScript
- Monaco Editor

External dependencies:

```text
Monaco Editor 0.45.0
Google Fonts
```

Monaco Editor is loaded from:

```text
cdnjs.cloudflare.com
```

The interface itself does not require a backend server.

---

# Important Notes

## Internet Connection

Waggo loads Monaco Editor from a CDN.

Therefore, a network connection is normally required when loading the application for the first time.

If the Monaco CDN cannot be reached, the editor may not start.

## HTML Preview Security

HTML preview is rendered using a sandboxed iframe:

```html
<iframe
    sandbox="allow-scripts allow-modals allow-forms allow-popups">
</iframe>
```

This provides isolation between the preview and the main Waggo application.

Do not treat the preview as a security boundary for untrusted code.

## Saving

Waggo downloads files to your computer instead of uploading them to a server.

The browser controls the actual download location.

---

# Troubleshooting

## The editor does not load

Check your internet connection.

Monaco Editor is loaded externally, so the CDN must be reachable.

Also check the browser developer console for errors.

---

## The Preview button is disabled

The Run button is only enabled when the active document uses the HTML language.

Select:

```text
HTML
```

from the language selector.

---

## My settings disappeared

Browser storage may be unavailable or blocked.

Try:

- Using a normal browser tab instead of private browsing
- Checking browser storage permissions
- Reloading the page

---

## Keyboard shortcut does not work

Check:

```text
Settings → Keyboard Shortcuts…
```

The shortcut may have been changed or removed.

You can restore the default shortcuts with:

```text
Reset all to defaults
```

---

# Project Structure

The current version is intentionally distributed as a single file:

```text
waggo.html
```

Conceptually, it contains:

```text
waggo.html
│
├── HTML
│   ├── Splash screen
│   ├── Application shell
│   ├── Menu bar
│   ├── Toolbar
│   ├── Sidebar
│   ├── Editor
│   ├── Preview
│   ├── Status bar
│   ├── Command Palette
│   └── Settings
│
├── CSS
│   ├── Dark theme
│   ├── Light theme
│   ├── Contrast theme
│   └── UI styles
│
└── JavaScript
    ├── OS detection
    ├── Storage
    ├── Command system
    ├── Keyboard shortcuts
    ├── Monaco initialization
    ├── Tabs
    ├── Preview
    ├── Themes
    ├── Command Palette
    └── Settings
```

---

# Credits

Waggo is built around the Monaco Editor.

The interface is designed to provide a lightweight, Kate-style coding experience directly in the browser.

---

# Version

```text
Waggo 0.1.0
```

> **code be freely**
