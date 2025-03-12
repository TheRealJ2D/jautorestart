# JAutoRestart

An advanced Minecraft server auto-restart plugin with lag detection and custom scheduling.

## Features

- 🕒 Scheduled restarts at specific times
- ⏰ Interval-based restarts
- 📊 TPS (Ticks Per Second) monitoring
- 🔄 Automatic restart on server lag
- ⚡ Inactivity-based restarts
- 🎮 User-friendly configuration GUI
- 🌐 BungeeCord support
- 🔔 Customizable notifications
- 📝 Fully configurable messages

## Commands

- `/jautorestart` - Shows help menu
- `/jautorestart restart [seconds]` - Initiates a server restart
- `/jautorestart cancel` - Cancels ongoing restart
- `/jautorestart reload` - Reloads configuration
- `/jautorestart gui` - Opens configuration GUI
- `/jautorestart update` - Checks for updates

## Permissions

- `jautorestart.admin` - Grants all permissions
- `jautorestart.restart` - Allows server restart
- `jautorestart.cancel` - Allows canceling restarts
- `jautorestart.reload` - Allows config reload
- `jautorestart.gui` - Allows GUI access
- `jautorestart.update` - Allows update checks

## Configuration

### config.yml
```yaml
scheduled_restarts:
  times:
    - "00:00"
    - "06:00"
    - "12:00"
    - "18:00"
  interval:
    enabled: false
    hours: 6

lag_detection:
  enabled: true
  threshold: 15.0
  check_interval: 60
  consecutive_checks: 3

inactivity_restart:
  enabled: true
  threshold_minutes: 30
