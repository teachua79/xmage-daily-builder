# Daily XMage Build

This repository hosts an **automated GitHub Actions workflow** that builds **daily snapshot releases** of [XMage](https://github.com/magefree/mage), the open-source Magic: The Gathering game engine.

## What it does

- Clones the official XMage repository daily.
- Builds the latest version of XMage using the `build-and-package.pl` script.
- Generates a timestamped binary ZIP file.
- Publishes a **GitHub release** with the daily snapshot.
- Automatically cleans up old releases and tags (keeping the latest 100).

**Note:** This repository is only for automated snapshot builds. There is **no support** provided here. If you encounter issues or have questions about XMage itself, please refer to the main repository.

## Workflow Schedule

The GitHub Actions workflow is scheduled to run **every day at 6:00 PM UTC**.  

**Note:** GitHub Actions schedules are subject to runner availability. Delays or skipped runs may occur occasionally. Releases depend on GitHub’s workflow execution and may not happen exactly on schedule.

## Important Notes

- These builds are **daily snapshots** for testing only.
- They may contain **unfinished features**, **experimental changes**, or **instabilities**.
- May not be suitable for official play.

## Release Naming

- The release tag and binary filename follow the format:  
  `daily-YYYY-MM-DD-HHMM`  
  Example: `daily-2025-11-29-1830.zip`

## License

The source code and builds are from the official XMage repository: [XMage](https://github.com/magefree/mage). This repository contains **automation scripts only**.
