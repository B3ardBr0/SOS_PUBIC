# iOS Shortcuts Version Control

A GitHub-based version control system for iOS Shortcuts, enabling easy management and synchronization across multiple devices.

## Features
- Automatic version checking
- Cross-device synchronization
- Change tracking
- Update notifications
- Version history

## Setup
1. Clone repository
2. Update `shortcut-info.json` with your details
3. Install base shortcut from provided iCloud link
4. Update GitHub raw URL in shortcut to point to your repository

## Usage
1. Launch shortcut to check for updates
2. If update available, shortcut will prompt to install new version
3. Accept update to install latest version

## Publishing Updates
1. Edit shortcut in iOS
2. Share → Copy iCloud Link
3. Update `shortcut-info.json`:
   - Increment version
   - Update shortcutURL
   - Add changelog entry
4. Commit changes

## JSON Structure
```json
{
    "metadata": {
        "creator": {...},
        "license": "",
        "repository": ""
    },
    "shortcut": {
        "name": "",
        "version": "",
        "shortcutURL": ""
    },
    "changelog": [...]
}
```

## Contributing
Pull requests welcome. For major changes, open an issue first.

## Creator
Wilhelm Maritz