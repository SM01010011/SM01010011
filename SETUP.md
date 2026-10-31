# Manual setup

Repository: `SM01010011/SM01010011`

## Upload

1. Download and extract the ZIP.
2. Open your GitHub profile repository: https://github.com/SM01010011/SM01010011
3. Upload the **contents** of the extracted folder to the repository root. Do not upload the outer ZIP or create an extra nested folder.
4. Keep the directory structure exactly as shown:

```text
SM01010011/
├── README.md
├── SETUP.md
├── assets/
│   ├── matrix-hero.svg
│   └── matrix-divider.svg
└── .github/
    └── workflows/
        └── profile-assets.yml
```

5. Commit the upload to the default branch.

## Enable the contribution snake

1. Open **Settings → Actions → General**.
2. Under **Workflow permissions**, select **Read and write permissions** and save.
3. Open **Actions** and enable workflows if GitHub prompts you.
4. Select **Refresh Profile Assets** → **Run workflow** → **Run workflow**.
5. Wait for the run to finish successfully. It creates/updates the `output` branch with the light and dark snake SVGs.

The snake image will appear after the output branch has been published. The scheduled workflow refreshes it every 12 hours.

## Notes

- The README and local SVG banner/divider do not depend on GitHub Readme Stats or skill-icons servers.
- Shields.io is used for technology badges and repository counters.
- The contribution snake requires GitHub Actions to run successfully.
- External badge and footer image services can occasionally be unavailable; no third-party service can be guaranteed.
- The avatar in the banner is a stylized `SM` monogram, not a photo. Replace it only if you want to add a profile photo.
