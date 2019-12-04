# TailDiscord (for simple monitoring of text files + notifications)

## Usage

Replace the two variables inside the taildiscord bash script. You can receive a webhook URL by editing a channel on a discord server where you have administrative permissions.

## Customization

This is a very simple bash script for server log monitoring, and you should edit it first if you intend to use it. Currently, it filters every log message that contains verbose and sends everything else. You should replace this with something useful, for instance, alerts if an error was logged.

## Full uptime

There are various solutions if you would like the script to be running constantly. By far one of the most simplest ways, is probably editing the crontab.
Example line (crontab -e):
```
# Log tail webhook post
@reboot cd ̃̃~/service/ && sh ./taildiscord
```