## Note: This fork currently only supports the base S3-Box3, and not the version with additional sensors.
# ESP32-S3-Box3-Custom Firmware: Home Assistant Front-End
This is a fork of an existing project that makes further use of the ESP32-S3-Box3's touch screen capabilities along with Home Assistant's voice assistant feature "Assist". This introduces a reworked front-end that operates similar to the Home Assistant dashboard, simulating its UI to work in much the same way. Some changes to this version of the project includes the following:
- Entire UI revision; entities, scenes, media player(s), and settings now stylized as lovelace cards
- Entities are now grouped together (6 supported currently)
- Easier entity substituion from the substitutions line
- Swap between light mode and dark mode with a single switch
- Implementation of weather info on the idle/main page
- Screensaver includes active timer

# This fork is still being updated to include functionality to current features and the recent alarmo additions, so there may be bugs or other issues presented that still need fixing. For this reason, it is recommended to be used by those familiar with ESPHome for now.
This fork is only possible through the work done on the main project by BigBobbas, so be sure to show them support for their work. Additionally the instruction docs provided by them, and the ESPHome documentation.

# Noted issues that may occur / need additional testing
- Text may run past its card, looking how to limit by characters.
- Fresh install untested, recommended to install main project, then update YAML in ESPHome with this fork.
- Original text files still included, but looking to migrate to Home Assistant fonts (i.e. Roboto).
- Some aspects (i.e. media player states) dependent on specific attributes required by entity.
