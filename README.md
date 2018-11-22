# better-thermostat
A better thermostat card for Home Assistant Lovelace UI

## Installation

1. Download the repo as a zip or with git clone and store it in `www/better-thermostat/` in your configuration folder.
2. Configure Lovelace to load the card:
    ```
    resources:
      - url: /local/better-thermostat/card.js?v=1
        type: module
    ```

## Example usage:

```yaml
cards:
  - type: custom:thermostat-card
    entity: climate.my_room
    energy: sensor.fibaro_system_fgwpef_wall_plug_gen5_energy
    power: sensor.fibaro_system_fgwpef_wall_plug_gen5_power
```
