# Waybar Microphone and Camera Usage Indicator

A simple bash script that outputs "MIC" and "CAM" respectively if either is in use. Intended for use in Waybar as I could not find a suitable alternative.

The checks being used are hardcode to fit my setup, but I have left comments to indicate what needs to change between setups.

Waybar config.jsonc custom config to show in waybar.
```
"custom/webcam": {
        "exec": "$HOME/.config/waybar/mic-cam-usage-indicator.sh",
        "interval": 3,  // Update every 5 seconds
        "format": "{0} {1}",
	"escape": true
    },
```
