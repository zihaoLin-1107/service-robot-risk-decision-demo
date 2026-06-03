# GitHub Upload Commands

This file is a local upload checklist for creating a separate public demo repository.

## Recommended Flow

Create a clean copy outside the full project:

```bash
mkdir -p ~/Projects/github_demo_repos
SOURCE_DIR="$HOME/Projects/indoor_robot_project/public_demo_repo"
rsync -av --exclude='.git' "$SOURCE_DIR/" ~/Projects/github_demo_repos/service-robot-risk-decision-demo/
cd ~/Projects/github_demo_repos/service-robot-risk-decision-demo
git init
git add .
git commit -m "Initial public demo package"
git branch -M main
```

Then manually create a new GitHub repository:

```text
service-robot-risk-decision-demo
```

## SSH Remote

Replace `USERNAME` with your GitHub username:

```bash
git remote add origin git@github.com:USERNAME/service-robot-risk-decision-demo.git
git push -u origin main
```

## HTTPS Remote

Replace `USERNAME` with your GitHub username:

```bash
git remote add origin https://github.com/USERNAME/service-robot-risk-decision-demo.git
git push -u origin main
```

## Before Pushing

Run:

```bash
find . -maxdepth 3 -type f | sort
git status --short
```

Confirm:

- No full source code is included.
- No raw experiment logs are included.
- No raw label tables are included.
- No private drafting materials or contact strategy files are included.
- No open-source `LICENSE` file is included.
- `NOTICE.md` and `NO_OPEN_SOURCE_LICENSE.md` are present.
- `media/case_a_demo_video_compressed.mp4` is included.
- Large local video files are not included.

## Note

This command document uses `$HOME` instead of a machine-specific absolute path. Adjust `SOURCE_DIR` if your local project path is different.
