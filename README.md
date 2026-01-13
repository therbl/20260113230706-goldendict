# GoldenDict Configuration

[![Version](https://img.shields.io/badge/version-v1.0.0-blue)](https://github.com/voothi/20260106194644-goldendict-roaming-data)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A repository for tracking and managing user-specific configurations, styles, and settings for GoldenDict. This setup ensures that your dictionary environment is portable and version-controlled.

## Table of Contents
- [Description](#description)
- [Features](#features)
- [Project Structure](#project-structure)
- [Git Integration](#git-integration)
- [Kardenwort](#kardenwort)
- [License](#license)

---

## Description
This project maintains the `GoldenDict` application data directory under version control. It tracks the core configuration, custom styles, and provides a structured way to handle transient data like history and favorites through a curated `.gitignore`.

[Return to Top](#goldendict-configuration)

## Features
- **Versioned Configuration**: Track changes to `config` and other XML settings.
- **Custom Styles**: Centralized management of `.css` files in the `styles/` directory.
- **Smart Git Filtering**: Automatically ignores transient files (history, favorites) and timestamped backups.
- **Portable Setup**: Easily sync your GoldenDict environment across multiple machines.

[Return to Top](#goldendict-configuration)

## Project Structure
- `config`: The main configuration file for GoldenDict.
- `styles/`: Contains custom CSS files for tweaking the look and feel of dictionary entries.
- `index/`: (Ignored) Directory for regeneratable search indexes.
- `a/`: (Ignored) Directory containing timestamped automated backups.
- `crash/`: (Ignored) Crash dump reports.

[Return to Top](#goldendict-configuration)

## Git Integration
The project uses a specific `.gitignore` to keep the repository clean of user-specific or transient data:

```gitignore
# History & favorites (transient, user-specific)
.history/
# history
# favorites

# Backups
a/
*.bak
*.old
*.tmp
* [0-9][0-9][0-9][0-9][0-9][0-9][0-9][0-9]*
```

> [!NOTE]
> History and favorites are currently commented out in `.gitignore` as per user preference, but remain listed for easy toggling.

[Return to Top](#goldendict-configuration)

## Kardenwort Ecosystem

This project is part of the **[Kardenwort](https://github.com/kardenwort)** environment, designed to create a focused and efficient learning ecosystem.

[Return to Top](#table-of-contents)

## Related Projects
- [Deep Translator Scripts](https://github.com/voothi/20241122093311-deep-translator)
- [Argo Translate Scripts](https://github.com/voothi/20241121100211-argotranslate)
- [TTS Scripts](https://github.com/voothi/20231001193911-tts)
- [Kardenwort](https://github.com/voothi/20241223170748-kardenwort)
- [Piper TTS](https://github.com/voothi/20241206010110-piper-tts)

[Return to Top](#goldendict-configuration)

## License
MIT License. See LICENSE file for details.

[Return to Top](#goldendict-configuration)
