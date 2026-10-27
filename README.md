# AI Box: server installer

The installer for the AI Box server (the computer we call PC-A) on Windows, and short videos that walk through
setting it up and using it.

Монгол хэлээр: [README.mn.md](README.mn.md)

## Download

- **Installer:** [AIBox-HeadNode-Setup-Wizard.exe](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest/download/AIBox-HeadNode-Setup-Wizard.exe), the latest release. Every
  file is on the [Releases](https://github.com/AI-box-mongolia/ai-box-setup/releases/latest) page.
- **Guide videos** (captions in Mongolian), in the [videos](videos) folder and on the Releases page:
  0. [Downloading the files from GitHub](videos/AI-Box-guide-0-download-from-github.mp4) (2:17)
  1. [Setting up the server](videos/AI-Box-guide-1-server-setup.mp4) (3:29)
  2. [Installing on an employee's computer, and sharing a file](videos/AI-Box-guide-2-employee-computer.mp4) (3:08)
  3. [What to do when Windows warns](videos/AI-Box-guide-3-windows-warnings.mp4) (2:47)
  4. [Using the AI Box web page](videos/AI-Box-guide-4-web-page.mp4) (3:47)
  5. [Setting up the Telegram bot (optional)](videos/AI-Box-guide-5-telegram.mp4) (2:43)
  6. [Updating the server: running the installer again](videos/AI-Box-guide-6-rerun-installer.mp4) (1:22)

## What the server computer needs

Windows 10 22H2 or Windows 11, 8 GB of memory, 10 GB of free disk space, an internet connection, and an
administrator account. Keep it switched on and plugged in: the other computers reach AI Box through it.

## Install

1. Double-click the installer. If Windows shows *Windows protected your PC*, choose **More info → Run anyway**: the
   installer is not signed. When Windows asks whether to allow changes, choose **Yes**.
2. Choose the language (English, or Mongolian) and follow the steps. It takes 10 to 20 minutes, and the computer may
   restart once.
3. When the server is running, the wizard offers an optional **Telegram bot** page: paste the token of a bot made with
   @BotFather to send files to people on Telegram, or leave it empty to skip (the install is never affected, and you can
   set it up later). The option that lets people ask the bot for files is off unless you tick it: files then pass through
   Telegram's cloud. Video 5 shows it.
4. Save the web address and the passwords the last page shows: they are not shown again.
5. For the employees' computers, setup creates `C:\AIBox\AIBox-Agent-Setup.exe`. Copy it to each computer and run it
   there. It carries a key to your server, so do not share it publicly.

## Check the download

In PowerShell, in the folder that holds the file:

```powershell
Get-FileHash .\AIBox-HeadNode-Setup-Wizard.exe
```

The *Hash* it prints must be exactly the SHA-256 in the release notes.

## Docker Desktop

The server runs on Docker Desktop. Docker's terms require a paid subscription for organizations with more than 250
employees or more than USD 10 million in annual revenue.
