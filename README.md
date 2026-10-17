# Approach Coach (beta)

Approach Coach grades the instrument approaches you fly in X-Plane 12 against the FAA instrument rating ACS, the way an examiner would. Pick any published approach X-Plane knows, choose where to start and the weather, fly it, and get a grade sheet. It runs next to X-Plane 12 on a Mac or a Windows PC.

This page holds the beta downloads only. **Get the newest version under [Releases](https://github.com/jmw5430/approach-coach-beta/releases/latest).**

- **Mac:** `ApproachCoach-<version>-mac.dmg`, one file for both Apple Silicon and Intel Macs.
- **Windows:** `ApproachCoachSetup-<version>.exe`.

It is a beta and not signed yet, so your computer will ask you to confirm it once. A home X-Plane setup is not an FAA-approved training device: these approaches do not count toward instrument currency.

## Mac

1. Download the `.dmg` and open it. Drag **Approach Coach** to **Applications**, then open it from there.
2. The first time, macOS says Apple could not verify it. Click Done, then open **System Settings**, **Privacy & Security**, scroll down, and click **Open Anyway** (enter your Mac password if asked). Right-click, then Open, no longer works on current macOS.
3. If macOS asks whether Approach Coach may accept incoming network connections, click **Allow**. That is what lets a phone or tablet in.
4. The coach page opens in your browser. Approach Coach has no Dock icon: it runs in the background and the page is the whole app. Open the app again any time to bring the page back.

## Windows

1. Download the setup file and run it. It installs just for you, with no administrator password.
2. Windows shows a blue box, "Windows protected your PC". Click **More info**, then **Run anyway**.
3. Finish the installer. You get an **Approach Coach** entry in the Start menu, an optional desktop icon, and a tick box at the end, **Open Approach Coach now**.
4. When Windows Firewall asks, allow Approach Coach on **private networks**. That is what lets a phone or tablet in.

## After it opens

1. Look at the one-line bar under the strip at the top of the page.
   - If it says the GPS plugin was installed, you are set.
   - If it asks you to quit X-Plane and open Approach Coach again, do that. The plugin can only be installed while X-Plane is closed.
   - If it cannot find X-Plane, it offers a box: type or paste X-Plane's folder there.
2. Start X-Plane. The first time, open Approach Coach before X-Plane so the plugin can be installed; after that, any order works. The plugin adds no item to X-Plane's Plugins menu; that is normal. It is listed under Plugins, Plugin Admin, Enable/Disable as "Approach Coach GPS".
3. **Phone or tablet:** on the same Wi-Fi, type the **https** address shown at the top of the page ("Phone/iPad: https://...:8443") into the phone's browser. Not `localhost`: on a phone that means the phone itself. The browser warns once that the connection is not private; accept it (Safari: Show Details, then visit this website, then Visit Website). If the page stays blank after that, refresh it once. That address keeps the screen on while you fly. Tip: add the page to the iPad's Home Screen (Share, Add to Home Screen); the icon asks you to accept the certificate once more the first time, then opens straight to the coach. If your computer's Wi-Fi address changes, the coach makes a new certificate and the browser asks once again.
   On version 0.1.0 the address is not on the page: on a Mac find it in System Settings, Wi-Fi, Details, TCP/IP (IP address); on Windows in Settings, Network, your Wi-Fi, IPv4 address. Then type `https://` + that address + `:8443`.
4. **Something wrong?** Send Jim the log file. Hover the version number at the top of the page to see where it is. On a Mac it is `~/.approach-coach/logs/coach.log`; on Windows it is `%USERPROFILE%\.approach-coach\logs\coach.log`.
5. **To quit:** click **Quit Approach Coach** at the top of the page.

## Updating

Download the newest release and install it over the old one. Your flights, logbook and settings stay where they are.
