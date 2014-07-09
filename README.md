# autocapture

bash script to execute OS X `screencapture` tool. Images are saved to `~/Documents/captures`.

## Installation

Move the script into `/usr/local/bin`:

```bash
cp autocapture /usr/local/bin/autocapture
```

Make executable:

```bash
chmod +x /usr/local/bin/autocapture
```

## Setup Capture Interval

Open the crontab:

```bash
EDITOR=nano crontab -e
```

Paste in the following to run the capture hourly:

```bash
0 * * * * /usr/local/bin/autocapture
```

To save:
ctrl o
enter

To close:
ctrl x

## Uninstall

Remove the autocapture script:

```bash
rm /usr/local/bin/autocapture
```

Open the crontab:

```bash
EDITOR=nano crontab -e
```

Remove the cronjob:

To delete the line added above:
ctrl k

To save:
ctrl o
enter

To close:
ctrl x