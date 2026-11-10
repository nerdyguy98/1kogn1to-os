# 1K0GN1T0 OS — Cloud ISO Build (fixed mirror configuration)

This starter builds a Debian 13 (Trixie) amd64 live ISO with KDE Plasma using GitHub Actions.

## Update an existing repository
Replace the existing `.github/workflows/build-iso.yml` with the one in this ZIP. Keep the `.github` folder and its workflow path intact.

## Run
1. Open your GitHub repository → Actions.
2. Select **Build 1K0GN1T0 OS ISO**.
3. Select **Run workflow** if available, or push a commit to main.
4. Open the latest run and wait for it to finish.
5. Download **1K0GN1T0-OS-amd64-ISO** if successful.

This is an early Debian-based prototype, not yet the finished branded desktop. The custom dock, launcher, control center, boot animation/chime and final artwork still need implementation and testing. Wine cannot guarantee every Windows program will work. No ISO exists until a workflow run succeeds.


Important: this workflow explicitly forces `--mode debian` and ignores host live-build defaults. This prevents the Ubuntu GitHub runner from configuring Ubuntu repositories for the Debian Trixie image.
