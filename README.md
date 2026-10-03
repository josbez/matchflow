<img src="icon.png" width="128" alt="Matchflow">

# Matchflow

A Mac menu bar app that shows at a glance how your club's match is going: home · score · away, with a bar showing who is on top right now. Click it for the match flow, the other live matches and the live table.

This repository holds the releases only.

## Install

Requires macOS 15 Sequoia or later (Apple Silicon and Intel).

1. **[Download Matchflow.dmg](https://github.com/josbez/matchflow/releases/latest/download/Matchflow.dmg)** (always the latest version; older versions and release notes are on the [releases page](https://github.com/josbez/matchflow/releases)) and open it.
2. Drag **Matchflow** to the **Applications** folder in the same window.
3. Open Terminal and run:

   ```bash
   bash /Volumes/Matchflow/install.sh
   ```

   This removes the Gatekeeper quarantine flag and installs a LaunchAgent, so Matchflow starts at login. Double-clicking `install.sh` does not work: macOS blocks it because the app is not notarised by Apple.
4. Choose your club or country. Its match then shows in the menu bar; allow notifications to get a heads-up on goals and red cards.

The app follows your macOS language: Dutch if that is your first preferred language, English otherwise.

## Updating

The app checks daily for a new version. If there is one, the gear in the popover gets a dot and you get a notification. Open settings and click **Update**: the app downloads the update, verifies its signature, replaces itself and restarts. Updates without a valid signature are rejected.

## Uninstall

Settings › **Uninstall…** removes the app, its LaunchAgent and its own files.

## Licence

[MIT](LICENSE)
