# GS HID Script Tool

**A Free Keyboard & Mouse Automation Learning Tool by GhostStrats**

## What Is GS HID Script Tool?

GS HID Script is a free educational application designed to help people learn how keyboard and mouse automation works.

The program was created by GhostStrats to make HID-style scripting easier to understand, especially for beginners who have little or no programming experience.

GS HID Script uses its own simple, human-readable scripting language. Instead of memorizing complicated commands, users can create scripts using plain English instructions.

The program allows you to:

- Learn how automated keyboard and mouse actions work.
- Write your own GS HID scripts.
- Create scripts with a visual builder.
- Simulate and preview scripts before running them.
- Execute scripts on your own computer for hands-on learning.
- Convert supported scripts between GS HID Script and DuckyScript.
- Learn keyboard shortcuts, delays, mouse movements, and scripting fundamentals.

**This is more than a script editor. It is an interactive learning environment where you can build, understand, preview, and test automation in one place.**

GS HID Script is free to download and use. No subscription, account, or internet connection is required to run the application.

---

## Main Features

### 1. GS HID Script Language

GS HID Script uses readable commands designed for beginners.

For example:

```text
PRESS WINDOWS + R
WAIT 1 SECOND
TYPE "notepad"
PRESS ENTER
WAIT 2 SECONDS
TYPE "Hello from GS HID Script!"
```

This script opens Windows Notepad and types a message.

Every command represents a specific action, making it easier to understand what the computer is being instructed to do.

### 2. Visual Script Builder

Don't know how to write scripts? No problem.

The Visual Builder allows you to create scripts through the interface without manually typing every command.

You can add actions such as:

- Typing text
- Pressing keyboard keys
- Performing keyboard shortcuts
- Adding delays
- Moving the mouse
- Clicking mouse buttons
- Scrolling

As you add actions, GS HID Script generates the corresponding code.

This helps beginners understand how visual actions translate into scripting commands.

The builder also includes convenient Windows examples for opening Notepad, Chrome, Command Prompt, PowerShell, and websites.

### 3. GS HID Script Lab

The Script Lab is where you create, edit, save, and test your scripts.

Features include:

**Script Editor:** Write and modify GS HID Script commands.

**Load Beginner Example:** Automatically load a simple practice script.

**Explain My Script:** Understand what each line of your script does.

**Step Through Preview:** Review the order of actions without sending real keyboard or mouse input.

**Execute Script:** Test your script using real keyboard and mouse automation on your computer.

**Open and Save:** Save scripts as `.gs` files and open them again later.

The Script Lab is designed to provide a learning environment where users can experiment and understand how automation works.

### 4. DuckyScript Converter

GS HID Script includes a built-in two-way DuckyScript converter.

Supported directions:

- GS HID Script to DuckyScript
- DuckyScript to GS HID Script

Paste your script into the converter, choose the direction, and click Convert.

The application translates supported commands and provides an output you can copy or save.

This feature is useful for learning the similarities and differences between scripting languages.

**Note:** Not every DuckyScript command is supported. The converter reports unsupported instructions rather than silently ignoring them. Some GS Script features, including mouse actions, cannot be represented in the basic DuckyScript output.

### 5. Built-In Learning Center

GS HID Script includes a learning section designed for beginners.

Learn about:

- Keyboard automation
- Mouse automation
- Scripting fundamentals
- Common key bindings
- Keyboard shortcuts
- Timing and delays
- Script execution
- Supported commands

The goal is to make scripting understandable without requiring previous cybersecurity or programming experience.

### 6. Script Safety Switch

GS HID Script includes a built-in Safety Switch to help prevent accidental script execution.

**Safety ON:** Scripts cannot execute.

**Safety OFF:** Script execution is available after the required confirmation.

The Safety Switch starts ON by default.

Before running a script, users must acknowledge that they are authorized to test the computer.

The application also provides a Stop function. On Windows, F12 can request an emergency stop.

A stop request cannot reverse actions already completed.

### 7. Custom GhostStrats Interface

GS HID Script features a black-and-purple GhostStrats interface.

Additional features include:

- Optional Glitch Mode
- Animated digital effects
- Custom GhostStrats artwork
- Hidden Easter egg
- Local browser-based interface
- Disconnect button to shut down the application

Glitch Mode and the Easter egg are visual features and do not execute automation commands.

---

## How GS HID Script Works

GS HID Script combines a beginner-friendly scripting language with a local automation engine.

When you create a script, the application reads each instruction and determines which keyboard or mouse action it represents.

You can first review the script using the explanation and preview features.

When you choose to execute it, GS HID Script sends the supported input actions to your computer through the operating system's automation capabilities.

For example, the command:

```text
TYPE "Hello World"
```

Tells the application to simulate typing Hello World into the currently focused window.

The command:

```text
PRESS CTRL + S
```

Simulates pressing Ctrl and S together.

And:

```text
WAIT 2 SECONDS
```

Tells the program to pause for two seconds before continuing.

**Technical information:**

- Windows uses the native `SendInput` API.
- Linux input playback uses `xdotool` under X11.
- macOS uses operating-system automation features and requires appropriate permissions.

The application runs locally on your computer and opens its interface in your web browser. The browser communicates with the locally running program; it does not require an online server.

---

## Download GS HID Script

Open the **Releases** section of this GitHub repository and download the version for your operating system.

**Available downloads:**

- `GS-HID-Script-Windows.zip` — Windows 10/11 (64-bit)
- `GS-HID-Script-Linux.zip` — Linux (64-bit)
- `GS-HID-Script-Mac-Apple.zip` — macOS Apple Silicon
- `GS-HID-Script-Mac-Intel.zip` — macOS Intel

These are portable applications, so there is no traditional installer.

The current executables are unsigned and may be restricted by operating-system security policies. Do not disable security protections to force them to run.

---

## Installation — Windows

1. Download `GS-HID-Script-Windows.zip`.
2. Right-click the downloaded ZIP.
3. Select **Extract All**.
4. Open the extracted folder.
5. Double-click `GS-HID-Script.exe`.
6. The application will open in your default browser.

That's it!

No Python, additional scripting software, or special keyboard drivers are required.

---

## Installation — Linux

Download and extract:

`GS-HID-Script-Linux.zip`

GS HID Script requires `xdotool` for actual keyboard and mouse playback on an X11 desktop.

On Debian, Ubuntu, or Linux Mint, install it using:

```bash
sudo apt update
sudo apt install xdotool
```

Open a terminal inside the extracted folder.

Give the application permission to execute:

```bash
chmod +x GS-HID-Script
```

Launch it:

```bash
./GS-HID-Script
```

The application will open its interface in your browser.

**Linux notes:**

The learning tools, visual builder, script editor, and converter can be used without `xdotool`.

Actual keyboard and mouse playback currently requires X11. Wayland playback is not supported in this release.

---

## Installation — macOS

Download the version for your Mac:

**Apple Silicon:** `GS-HID-Script-Mac-Apple.zip`

**Intel:** `GS-HID-Script-Mac-Intel.zip`

Extract the ZIP.

Open Terminal inside the extracted folder and run:

```bash
chmod +x GS-HID-Script
./GS-HID-Script
```

GS HID Script will open in your browser.

For real automation, macOS requires Accessibility permissions under System Settings → Privacy & Security → Accessibility.

Some mouse functions require the optional `cliclick` utility, and automation features are more limited than on Windows.

These Mac builds are unsigned and may be blocked by Gatekeeper. Do not disable security protections to force execution.

---

## How to Use GS HID Script

### Step 1 — Launch the application

Open GS HID Script using the instructions for your operating system.

The interface will appear in your default browser.

### Step 2 — Explore the Learning Center

If you're new to scripting, start with the Learn section.

Explore the available commands, keyboard bindings, and examples.

### Step 3 — Create a script

Open the GS HID Script Lab.

You can write your own commands or load the beginner example.

You can also use the Visual Builder to generate scripts.

### Step 4 — Preview your script

Click **Explain My Script** to understand the instructions.

Use **Step Through Preview** to review the script without actually controlling your computer.

### Step 5 — Test your script

When you understand the script and are ready to test:

1. Use a computer you own or have permission to test.
2. Turn the Safety Switch OFF.
3. Check the authorization confirmation.
4. Click Execute.
5. Approve the execution confirmation.
6. Focus your intended test application during the countdown.

The program will execute the supported instructions.

**Important:** Real automation acts on the currently focused application. Test with harmless scripts and review every action first.

---

## Your First GS HID Script

Try this simple example on Windows.

```text
# Open Windows Notepad

PRESS WINDOWS + R
WAIT 1 SECOND
TYPE "notepad"
PRESS ENTER
WAIT 2 SECONDS

# Type a message

TYPE "Hello from GS HID Script!"
PRESS ENTER
TYPE "Safety is an Illusion."
PRESS ENTER
```

### What does this script do?

1. Opens the Windows Run dialog.
2. Waits one second.
3. Types `notepad`.
4. Presses Enter to launch Notepad.
5. Waits two seconds for Notepad to open.
6. Types a message.
7. Presses Enter.
8. Types a second message.

This demonstrates keyboard shortcuts, text entry, delays, and automated execution.

If Notepad takes longer to open, increase the delay.

---

## GS HID Script Commands

### Type Text

```text
TYPE "Hello World"
```

Types text into the active window.

Quotation marks are optional for ordinary text.

### Press a Key

```text
PRESS ENTER
PRESS TAB
PRESS ESC
```

### Keyboard Shortcuts

```text
PRESS CTRL + C
PRESS CTRL + V
PRESS CTRL + S
PRESS WINDOWS + R
```

### Add a Delay

```text
WAIT 1 SECOND
WAIT 5 SECONDS
WAIT 500 MILLISECONDS
```

### Move the Mouse

```text
MOVE MOUSE TO 500, 300
```

Moves the mouse pointer to a specified screen position.

### Mouse Clicks

```text
CLICK LEFT
CLICK RIGHT
```

### Scrolling

```text
SCROLL UP 3
SCROLL DOWN 3
```

### Comments

```text
# This line is a comment
```

Comments explain your script and do not execute.

The complete list of supported commands and keyboard bindings is available in the Learning Center and the included language guide.

---

## Saving and Sharing Scripts

GS HID Script allows users to save scripts as `.gs` files.

These files contain readable script instructions.

You can:

- Save scripts for future use.
- Open previously created scripts.
- Edit and improve your scripts.
- Share examples with other learners.
- Convert supported scripts to DuckyScript.

Always review scripts from other people before executing them.

---

## How to Stop or Disconnect

To stop a running script, click **Stop** or turn the Safety Switch ON.

On Windows, you can also press F12 to request an emergency stop.

To disconnect the application:

1. Click **Disconnect GS HID Script from This Computer**.
2. Confirm the request.
3. Wait for the Disconnected confirmation.
4. Close the browser tab.

This shuts down the local GS HID Script program.

---

## How to Uninstall

GS HID Script is a portable application.

There is no traditional installer or separate uninstaller.

To remove GS HID Script:

1. Disconnect the application.
2. Close any remaining running GS HID Script process.
3. Delete the extracted application folder.
4. Delete the downloaded ZIP if no longer needed.

Any separately saved `.gs` files will remain wherever you saved them.

Utilities installed separately, such as `xdotool`, are not automatically removed.

---

## For Developers and Hardware Manufacturers

GS HID Script includes a Universal Vendor Converter Kit.

This allows independent developers and manufacturers to create compatible translators for their own scripting platforms.

The kit includes:

- Language specifications
- Command definitions
- Reference parser
- JSON action format
- Conversion examples
- Compatibility tests

Independent vendor integrations are not official GhostStrats products unless explicitly authorized.

See the vendor converter documentation for implementation details and applicable licensing terms.

---

## Educational Purpose and Disclaimer

GS HID Script is developed and distributed free of charge by **GhostStrats LLC** for cybersecurity education, awareness, defensive research, and authorized testing.

This project is intended to help people learn how automation works through a beginner-friendly environment.

Users are responsible for reviewing their scripts, obtaining any necessary permissions, and following applicable laws.

GhostStrats LLC does not endorse illegal activities, unauthorized access, or malicious use of this software.

**GS HID Script is provided "AS IS," without warranties of any kind.**

To the maximum extent permitted by applicable law, GhostStrats LLC and its contributors disclaim liability for damage, data loss, misuse, unauthorized activity, independent modifications, or third-party integrations.

See `LICENSE` and `DISCLAIMER.md` for the complete terms.

---

## License

Copyright © 2026 GhostStrats LLC.

GS HID Script is provided under the **GS HID Script Free Educational Software License v1.0**.

The software is free to use, study, modify, and share under the included license terms.

Redistributed versions of the application must remain free and clearly identify independent modifications.

GS HID Script uses a custom source-available license rather than the MIT License.

---

## About GhostStrats

GhostStrats focuses on cybersecurity education, privacy awareness, defensive technology, Linux, and helping people better understand the systems they use every day.

The purpose of GS HID Script is to make technical knowledge more accessible by providing a free learning tool that people can explore at their own pace.

**Knowledge should be accessible. Learning should be encouraged.**

Created by **GhostStrats LLC**

**SAFETY IS AN ILLUSION.**
