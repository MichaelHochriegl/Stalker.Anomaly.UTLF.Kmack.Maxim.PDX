# Universal Tactical Light Framework - Kmack Maxim PDX Patch

Compatibility patch for `Universal Tactical Light Framework` and `[Kmack] Maxim PDX and Optics Package`.

## Requirements

- [Universal Tactical Light Framework](https://github.com/MichaelHochriegl/Stalker.Anomaly.Universal.Tactical.Light.Framework)
- [Kmack] Maxim PDX and Optics Package
- Anomaly/GAMMA with Modded Exes support for `attachment_script_light`

## Supported Sections

- `wpn_pdx`
- `wpn_pdx_terminal`
- `wpn_pdx_terminal_off`

## MCM

This patch adds a nested page under `Universal Tactical Light Framework` > `Kmack Maxim PDX`.

Configurable values:

- `Light range`: defaults to `26`, configurable from `5` to `80`.
- `Cone angle`: defaults to `24`, configurable from `8` to `60` degrees.

Changing these values re-registers the PDX light profile. If the PDX light is currently active, the framework reattaches it with the new values.

The patch uses `utlf.setup_configured_pack()` with the `kmack_pdx` MCM namespace, so these values are stored separately from other weapon patch mods.


## Installation

Install as its own MO2 mod and load it after the framework and after the Maxim PDX package.

Recommended order:

1. `[Kmack] Maxim PDX and Optics Package`
2. `Universal Tactical Light Framework`
3. `Universal Tactical Light Framework - Kmack Maxim PDX Patch`
