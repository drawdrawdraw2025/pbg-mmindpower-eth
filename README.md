# pbg-mmindpwer-free - Filebase IPFS Auto Deploy

This repo auto-deploys to **Filebase IPFS** on every push to `main`.

- Workflow: `.github/workflows/ipfs-deploy.yml`
- Bucket: `pbg-mmindpwer-free`
- Service: Filebase via `aquiladev/ipfs-action@v0.3.2`
- Pin: `true`

## How it works
1. You push code to `main` branch on GitHub
2. GitHub Actions runs the workflow
3. Action uploads `./` to Filebase bucket `pbg-mmindpwer-free`
4. Filebase pins it to IPFS (using FILEBASE_KEY and FILEBASE_SECRET secrets)

Secrets required in GitHub repo: `FILEBASE_KEY` and `FILEBASE_SECRET`
Crust auto-pin enabled 2026-09-27T06:17:59Z
