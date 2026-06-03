# Create GitHub Release

Use this only after the public demo repository has been checked for sensitive files and large raw artifacts.

Do not upload raw logs, the main project source, raw labels, SOP materials, advisor lists, or prompts.

## Option A: GitHub Website

1. Go to the repository's **Releases** page.
2. Click **Draft a new release**.
3. Tag: `phd-application-demo-v0.1`
4. Title: `PhD Application Demo v0.1`
5. Paste the content from `RELEASE_NOTES_v0.1.md`.
6. Attach `media/case_a_demo_video_compressed.mp4` if desired.
7. Publish the release.

## Option B: GitHub CLI

```bash
gh release create phd-application-demo-v0.1 \
  media/case_a_demo_video_compressed.mp4 \
  docs/01_Project_Brief_EN.pdf \
  docs/02_Project_Brief_ZH_Visual.pdf \
  --title "PhD Application Demo v0.1" \
  --notes-file RELEASE_NOTES_v0.1.md
```

## Reminder

- Do not upload raw logs.
- Do not upload the main project source.
- Do not upload raw labels.
- Do not add an open-source license unless the repository scope changes.

