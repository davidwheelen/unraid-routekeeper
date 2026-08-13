# RouteKeeper for Unraid

RouteKeeper is a native Unraid WebGUI plugin for saving selected static routes and restoring them automatically after boot.

It is intended for administrators who want persistent IPv4 or IPv6 routes without maintaining shell commands, startup scripts, or Docker containers.

## Install

Use this plugin installer URL in Unraid:

```text
https://raw.githubusercontent.com/davidwheelen/unraid-routekeeper/main/routekeeper.plg
```

In the Unraid WebGUI, install the plugin from the Plugins page by pasting the URL above into the install plugin field.

After installation, open:

```text
Settings -> RouteKeeper
```

## What RouteKeeper Does

- Shows live IPv4 and IPv6 routes from Unraid's routing table.
- Lets you explicitly save selected routes for persistence using right-side checkboxes.
- Restores enabled saved routes after Unraid starts.
- Lets you temporarily remove a live route without deleting its saved definition.
- Provides a master switch for automatic restoration.

RouteKeeper does not replace Unraid Network Settings, does not edit `network.cfg`, and does not blindly persist the whole routing table.

## Supported Version

- Minimum Unraid version: 7.2.0
- RouteKeeper version: 2026.08.23

## Files In This Repository

This repository hosts the public installer files required for Unraid installation:

- `routekeeper.plg`
- `routekeeper-2026.08.23-noarch-1.txz`
- `routekeeper-2026.08.23-noarch-1.txz.sha256`
- `plugins/routekeeper.xml`
- `assets/routekeeper.svg`

The development source tree is not published in this repository.

## Support

Use GitHub Issues in this repository for installation problems, bug reports, and compatibility feedback.

## License

MIT
