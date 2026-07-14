# Push NFA to GitHub

Your code is committed **locally** on branch `main`. It is not on GitHub until you complete the steps below.

## Step 1 — Repository

Remote already exists:

**https://github.com/Manjith-NG/NFA-2.0-Ver**

## Step 2 — Push from your PC

Open PowerShell in this folder:

```powershell
cd "c:\Users\Manjith\Downloads\NFA-2.0-Ver"
.\scripts\push-github.ps1
```

Or manually:

```powershell
cd "c:\Users\Manjith\Downloads\NFA-2.0-Ver"
git add -A
git commit -m "Update project files"   # only if there are changes
git push -u origin main
```

When Windows asks you to sign in:

- Choose **Sign in with your browser**, or  
- Use a **Personal Access Token** as the password  
  - Create at: https://github.com/settings/tokens  
  - Enable scope: **repo**

## Step 3 — Verify

Open: **https://github.com/Manjith-NG/NFA-2.0-Ver**

You should see all project files (README, `src/`, `prisma/`, etc.).

## Troubleshooting

| Problem | Fix |
|--------|-----|
| `Repository not found` | Confirm the repo exists at https://github.com/Manjith-NG/NFA-2.0-Ver |
| `Authentication failed` | Sign in again via Git Credential Manager or use a PAT |
| `failed to push — rejected` | Remote has commits: run `git pull origin main --rebase` then push again |
| `remote origin already exists` | Remote is fine; just run `git push -u origin main` |

Remote URL:

```
https://github.com/Manjith-NG/NFA-2.0-Ver.git
```
