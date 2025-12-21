
`systemctl` is the command-line tool to control **systemd**, the init system and service manager used by many modern Linux distros (e.g., Fedora, Ubuntu, Arch, Debian).  
It starts/stops/enables/disables services (a.k.a. _units_), reloads configs, and queries system state.

| Command                               | Meaning                                        |
| ------------------------------------- | ---------------------------------------------- |
| `sudo systemctl start name.service`   | Start a service now                            |
| `sudo systemctl stop name.service`    | Stop a service now                             |
| `sudo systemctl restart name.service` | Stop then start (hard restart)                 |
| `sudo systemctl reload name.service`  | Tell service to reload config (graceful)       |
| `sudo systemctl enable name.service`  | Start at boot (enable unit)                    |
| `sudo systemctl disable name.service` | Do not start at boot                           |
| `sudo systemctl status name.service`  | Show status + logs snippet                     |
| `systemctl is-enabled name.service`   | Is it enabled at boot? (yes/no)                |
| `systemctl list-units --type=service` | List active services                           |
| `systemctl list-unit-files`           | List known unit files and enabled/disabled     |
| `sudo systemctl daemon-reload`        | Reload unit files after editing                |
| `sudo systemctl mask name.service`    | Prevent a unit from being started              |
| `sudo systemctl unmask name.service`  | Re-enable a masked unit                        |
| `sudo systemctl edit name.service`    | Create drop-in override (recommended)          |
| `systemctl show name.service`         | Low-level properties of a unit                 |
| `journalctl -u name.service`          | Show full logs for the service (use with sudo) |