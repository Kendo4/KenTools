# KenTools - Steam Plugin

A powerful Steam plugin for managing game fixes, scripts, and more.

## Overview

KenTools is a Steam plugin built for the Millennium framework, providing tools for managing game fixes, scripts, and various utilities.

## Installation

1. Extract the plugin to your Steam plugins directory:
   ```
   Steam/plugins/kentools/
   ```

2. Restart Steam to load the plugin

3. The plugin will appear in your Steam interface

## Building

### Windows (PowerShell)

```powershell
# Basic build
.\build.ps1

# Build with cleanup
.\build.ps1 -Clean

# Custom output name
.\build.ps1 -OutputName "kentools-v1.0.zip"
```

### Linux/Mac (Bash)

```bash
# Make executable (first time)
chmod +x build.sh

# Execute
./build.sh

# With cleanup
./build.sh kentoolsplugin.zip true
```

## Project Structure

```
KenTools/
├── backend/          # Python backend code
│   ├── locales/     # Translation files
│   └── settings/    # Settings management
├── public/          # Frontend assets
│   ├── kentools.js  # Main JavaScript file
│   └── kentools-icon.png  # Plugin icon (replace with your logo)
├── scripts/         # Build and validation scripts
├── plugin.json      # Plugin manifest
├── requirements.txt # Python dependencies
└── build.ps1        # Windows build script
```

## Customization

### Logo/Icon

Replace `public/kentools-icon.png` with your own logo. The recommended size is 64x64 pixels or larger (PNG format).

### Branding

All references to "KenTools" and "kentools" can be customized by:
1. Updating `plugin.json` (name, common_name, description)
2. Running the rebranding script (if you create one) or manually replacing strings
3. Updating the icon file

## Development

### Requirements

- Python 3.x
- Millennium Steam framework
- httpx==0.27.2
- requests

### Dependencies

Install Python dependencies:
```bash
pip install -r requirements.txt
```

## License

This project is based on LuaTools. Please ensure you comply with any original licensing terms and create your own unique implementation.

## Notes

- Replace `public/kentools-icon.png` with your own logo
- Update `backend/update.json` with your own GitHub repository if you want auto-updates
- Customize API endpoints and URLs in `backend/config.py` as needed
- Review and update locale files in `backend/locales/` for your branding

## Support

For issues and questions, please refer to your project repository.

