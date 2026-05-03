# Cam5Raspi

A collection of Python scripts for working with cameras on the Raspberry Pi 5.

## camera_preview.py

Displays a live preview window from an **IMX219** camera attached to **cam0**
on a Raspberry Pi 5.  The window stays open until you press **Ctrl+C**.

### Requirements

| Requirement | Notes |
|---|---|
| Raspberry Pi 5 | Any memory variant |
| IMX219 camera module | Connected to the **cam0** ribbon-cable connector |
| Raspberry Pi OS (Bookworm or later) | 64-bit recommended |
| `picamera2` | Pre-installed on Raspberry Pi OS; install with `sudo apt install -y python3-picamera2` if missing |
| Qt display libraries | `sudo apt install -y python3-pyqt5` |

### Usage

```bash
# Run directly
python3 camera_preview.py

# Or make it executable first
chmod +x camera_preview.py
./camera_preview.py
```

Press **Ctrl+C** in the terminal to close the preview window and stop the camera.
