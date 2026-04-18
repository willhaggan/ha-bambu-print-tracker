# Bambu Lab Print Status and Energy Tracker

A Home Assistant blueprint to monitor Bambu Lab 3D prints. This blueprint provides monitoring for print progress, completion, and failures, with integrated cost and energy tracking.

<a href="https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fwillhaggan%2Fha-bambu-print-tracker%2Fblob%2Fmain%2Fbambu_update_main.yaml" target="_blank" rel="noreferrer noopener"><img src="https://my.home-assistant.io/badges/blueprint_import.svg" alt="Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled." /></a>

---

## Features
- **Real-Time Progress:** Monitor completion percentage with adjustable update intervals.
- **Cost Calculation:** Calculate filament and energy costs per print job.
- **Energy Tracking:** Integration for smart plugs with kWh sensors and support for dynamic electricity pricing.
- **Visual Feedback:** Support for live camera snapshots or cover images within notifications.
- **Smart Snooze:** Interactive mute functionality allowing users to silence updates for a specific duration via text input.
- **Quiet Hours:** Optional schedule to silence progress updates during specified time windows. Critical alerts (Completion/Failure) bypass this setting.

## Requirements
The following components are required for full functionality:
1. **Bambu Lab Integration:** Installed via HACS or official methods.
2. **Mobile App Integration:** Required for actionable notifications.
3. **Helpers (Optional):**
   - An `input_datetime` (configured for Date and Time) is required for the Snooze feature.
   - An `input_number` is required to store the starting kWh for energy tracking.

## Installation
1. Click the Import Blueprint button above or copy the URL of the YAML file.
2. In Home Assistant, navigate to Settings > Automations & Scenes > Blueprints.
3. Click Import Blueprint and paste the URL.
4. Create an automation from the imported blueprint and map your printer sensors to the inputs.

---

## Contributing
For bug reports or feature requests, please open an issue in this repository.
