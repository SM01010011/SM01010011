# Profile setup

## 1. Create the profile repository

Create a **public** GitHub repository named exactly `SM01010011` (your GitHub username). Add a README if the repository is new.

## 2. Upload the files

Upload the contents of this project while preserving this structure:

```text
.
├── .github/
│   └── workflows/
│       └── profile.yml
├── assets/
│   ├── banner.svg
│   ├── footer.svg
│   ├── strip-moveset.svg
│   ├── strip-skypillar.svg
│   └── strip-trainer.svg
├── README.md
└── SETUP.md
```

## 3. Enable workflow permissions

Open **Settings → Actions → General → Workflow permissions**, select **Read and write permissions**, and save.

## 4. Run the profile workflow

Open **Actions → Profile animations → Run workflow**. The workflow generates the 3D contribution graph and publishes the contribution snake to the `output` branch. It also runs on the configured daily schedule and when you push to `main`.

## 5. Check your profile

Refresh `https://github.com/SM01010011`. The generated contribution images may take a few minutes to appear after the first run.

## Notes

- The profile artwork is stored in `assets/`; keep those paths unchanged unless you also update the README image references.
- GitHub-hosted SVG animations and third-party stats services can occasionally load slowly or be temporarily unavailable.
- Pokémon artwork and names belong to their respective rights holders. This fan-made profile is non-commercial.
