
# ASTRO Blackstar [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/siryasko) 



Web control panel for a **Blackstar ID Core** amplifier, driven over
**WebHID** straight from the browser — no drivers, no companion app.

## Supported amplifiers

Right now only **ID:Core Stereo 10 V4** and **ID:Core Stereo 40 V1** are
confirmed working (their USB VID/PID are known). Other models/generations in
the ID:Core Stereo line may or may not work yet.

If you have a different model and it doesn't connect, please get in touch
with your amp's **USB VID/PID** so it can be added:
- **Windows:** Device Manager → Properties → Details → Hardware Ids
- **macOS:** About This Mac → More Info → System Report → USB (left
  sidebar) → select the amp's entry → **Product ID** / **Vendor ID**. This
  is the most reliable way. In Terminal, `system_profiler SPUSBDataType`
  works on older macOS versions; on newer ones the same data is under
  `system_profiler SPUSBHostDataType` instead (Apple renamed it) — if one
  prints nothing, try the other.
  Search for an entry similar to the one below:
  ```
  ID:Core v4:
     Location ID: 0x02000000
     Connection Type: Removable
     Manufacturer: Blackstar Amplification Limited
     Serial Number: Not Provided
     Link Speed: 480 Mb/s
     USB Vendor ID: 0x27d4
     USB Product ID: 0x0013
     USB Product Version: 0x0098
  ```


## Usage

1. Run latest version directly from [GitHub](https://siryasko.github.io/ASTRO-Blackstar/astro-blackstar.html)

    or
2. Download [`astro-blackstar.html`](https://siryasko.github.io/ASTRO-Blackstar/astro-blackstar.html) and open it in a WebHID-capable browser (Chrome/Edge)
3. Connect the amp over USB and click **USB switch** to pair it via WebHID.

## Features

- Full amp control: voice, gain, volume, EQ, effects (MOD/DLY/REV), noise
  gate, USB settings
- Presets: save/load/import/export, switch with a single click or by pressing the preset's number key
- Built-in metronome and microphone pitch tuner (work without the amp
  connected)
- WAV recorder for the amp's USB audio output
- Raw HID console for low-level protocol experimentation

## Versioning

The bottom status strip shows a `VERSION` field stamped with the build's date/time (`YYYYMMDD.HHMM`), so you can tell which build you're
running.

## Contributing

If you have knowledge about these amplifiers or ideas for further development, feel free to reach out.

---

Author: **Sir Yasko** 

If you like this project and want to support my work, you can [buy me a coffee](https://www.buymeacoffee.com/siryasko) ☕

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/siryasko) 