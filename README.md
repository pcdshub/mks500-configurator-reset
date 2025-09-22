# mks500-configurator

For setting MKS500 gauges back to their default settings (LCLS-I config)

Just plug the gauge electronics into your Windows laptop with a USB micro cable and double-click the executable.

1. Reads every uncommented command/query from gauge, records as (save)
2. Executes each command with the argument. If the argument is NA, it is skipped. Change NA to value you want programmed. (resp)
3. Reads every command to confirm settings were accepted. (check)

To change settings:
- Edit the settings.cfg file. Change NA to the value you want programmed.

To build the exe
- install pyinstaller
- run 'pyinstaller mks500_configurator.spec'
- .exe will be available under ./dist
