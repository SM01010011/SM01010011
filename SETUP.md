# Setup your GitHub profile

This package is prepared for the profile repository `SM01010011`.

## Repository layout

Keep this structure when uploading the files:

```text
SM01010011/
├── README.md
├── assets/
│   ├── matrix-hero.svg
│   └── matrix-divider.svg
└── .github/
    └── workflows/
        └── profile-assets.yml
```

## Installation

1. Open https://github.com/new.
2. Create a **public** repository named exactly `SM01010011`.
3. Upload the contents of this package, preserving the folders shown above.
4. Commit the files to the repository's default branch (`main` is recommended).
5. Open **Settings → Actions → General**.
6. Under **Workflow permissions**, select **Read and write permissions**, then save.
7. Open the **Actions** tab and enable workflows if GitHub asks.
8. Run **Refresh Profile Assets** once using **Run workflow**.

The workflow has two jobs:
- It embeds your current GitHub avatar into `assets/matrix-hero.svg`.
- It generates light and dark contribution-snake SVGs and publishes them to the `output` branch.

After the first successful run, the snake image should appear in your profile README. Scheduled runs refresh the assets every 12 hours. Push-triggered runs are limited to changes in the hero SVG or workflow file, so ordinary README edits do not waste workflow runs. GitHub may automatically disable scheduled workflows in repositories with prolonged inactivity; run the workflow manually if that happens.

## Notes

- The profile repository name must match your GitHub username exactly.
- The workflow needs `contents: write` permission to update the banner and publish the `output` branch. The workflow validates the edited hero SVG before committing it and serializes runs to avoid overlapping output-branch publishes.
- The LinkedIn and email links in the README were retained from the files you supplied. Update them if either has changed.
- GitHub README rendering does not run JavaScript or arbitrary CSS. The animated elements use SVGs and external image services.
- GitHub statistics, contribution graphs, typing text and trophy cards depend on third-party services and may occasionally be unavailable.
