## Note: This fork currently only supports the base S3-Box3, and not the version with additional sensors.
# ESP32-S3-Box3-Custom Firmware: Home Assistant Front-End
This is a fork of an existing project that makes further use of the ESP32-S3-Box3's touch screen capabilities along with Home Assistant's voice assistant feature "Assist". This introduces a reworked front-end that operates similar to the Home Assistant dashboard, simulating its UI to work in much the same way. Some changes to this version of the project includes the following:
- Entire UI revision; entities, scenes, media player(s), and settings now stylized as lovelace cards
- Device entities are now grouped together (6 supported currently)
- Control 2 additional external media players
- Up to 12 scene entities supported
- Easier entity substituion from the substitutions line
- Swap between light mode and dark mode with a single switch
- Implementation of weather info on the idle/main page
- Screensaver includes active timer

## This fork is still being updated to include functionality to current features and the recent alarmo additions, so there may be bugs or other issues presented that still need fixing. For this reason, it is recommended to be used by those familiar with ESPHome for now.
This fork is only possible through the work done on the main project by BigBobbas, so be sure to show them support for their work. Additionally the instruction docs provided by them, and the ESPHome documentation.

# Images
![Main Page](https://github.com/user-attachments/assets/45ae11e5-aad6-48d8-98ca-38a261c0577b)
![Entity Page](https://github.com/user-attachments/assets/0e3c7a94-2988-49ed-ab6b-b92dcf1a5c61)
![Media](https://github.com/user-attachments/assets/3360aac5-af1b-469c-98a9-337fed76da80)
![Options   Dark Mode](https://github.com/user-attachments/assets/64fda766-1668-4639-be36-81b0d2e2cfe0)

# Noted issues that may occur / need additional testing
- Text may run past its card, looking how to limit by characters.
- Fresh install untested, recommended to install main project, then update YAML in ESPHome with this fork.
- Original text files still included, but looking to migrate to Home Assistant fonts (i.e. Roboto).
- Some aspects (i.e. media player states) dependent on specific attributes required by entity.
- Sidebar icons can still be accessed from screensaver. May update screensaver in later update.

# To work on (no particular order)
- Fix bugs outstanding
- ~~Update scenes page to allow more scene entities~~
- Implement icon autofill and bubble colors based on entity type
- Album artwork (is it possible?) on media player page
