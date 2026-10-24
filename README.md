# LumiKaka

Homepage: https://lumikaka.github.io/

The page source lives in [lumikaka/lumi/root-site](https://github.com/lumikaka/lumi/tree/master/root-site). This repository contains only the GitHub Pages publishing workflow.

## Publish

Open **Actions → Root Pages → Run workflow**. Use workflow branch `main` and source ref `master`, or select a Lumi source commit/tag to publish an earlier version. The workflow reads the public source and deploys it using this repository’s built-in GitHub credentials. No deploy key or personal token is needed.

```bash
gh workflow run root-pages.yml --repo lumikaka/lumikaka.github.io --ref main -f source_ref=master
```

The workflow source is maintained at [root-site/deploy/root-pages.yml](https://github.com/lumikaka/lumi/blob/master/root-site/deploy/root-pages.yml). When changing the deployment workflow, update that file and sync it to `.github/workflows/root-pages.yml` here.
