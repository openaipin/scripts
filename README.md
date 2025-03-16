## Installation and Usage
Clone the repo and ensure you have adb installed and your AI Pin is connected (see [Building an Interposer](https://github.com/MaxMaeder/OpenPin?tab=readme-ov-file#building-a-interposer))

```bash
git clone https://github.com/openaipin/scripts.git
cd scripts/scripts
```

Push scripts to the device (/data/local/tmp/openPin-scripts) and set execute permissions
```bash
adb push . /data/local/tmp/openPin-scripts
adb shell chmod +x /data/local/tmp/openPin-scripts/*.sh
```

To run a script:
```bash
adb shell
cd /data/local/tmp/openPin-scripts
./<script-name>.sh
```

## Available Scripts

|Enable|Disable|Description|
|-|-|-|
|`always_on_display_enable.sh`|`always_on_display_disable.sh`|Enables always-on display for debugging purposes, useful if you want to scrcpy without the need to hold your hand out. This can cause the Ai Pin to overheat. |
|`touch_indicator_enable.sh`|`touch_indicator_disable.sh`|Displays touch (click) indicators on-screen.|

## Contributing:
Submit issues, ideas, or contributions through GitHub issues or pull requests.