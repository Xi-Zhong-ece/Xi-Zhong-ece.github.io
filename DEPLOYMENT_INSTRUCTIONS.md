# Deploying the site

Target repository: `Xi-Zhong-ece/Xi-Zhong-ece.github.io`  
Target website: `https://xi-zhong-ece.github.io`

## Replace the current simple HTML site

1. Back up the current repository if you want to keep the old version.
2. Replace the current repository contents with **all files and folders in this package**, including the hidden `.github` folder.
3. In GitHub, open **Settings → Actions → General → Workflow permissions**.
4. Select **Read and write permissions**, then click **Save**.
5. Commit/push everything to the `main` branch.
6. Open the repository **Actions** tab and wait for **Deploy site** to finish successfully. This creates/updates the `gh-pages` branch.
7. Open **Settings → Pages**.
8. Under **Build and deployment**, select **Deploy from a branch**.
9. Set the branch to **gh-pages** and the folder to **/(root)**, then click **Save**.
10. Wait about a minute, then open `https://xi-zhong-ece.github.io`.

## Important on macOS

The `.github` folder is hidden in Finder. Press **Command + Shift + .** to show hidden files before uploading. Another reliable option is GitHub Desktop, which includes hidden files automatically.

If `.github/workflows/deploy.yml` is not in the repository, the al-folio site will not build.

## Updating the site later

- Homepage bio: `_pages/about.md`
- Research: `_pages/research.md`
- Publications: `_bibliography/papers.bib`
- News: add a dated Markdown file in `_news/`
- CV: replace `assets/pdf/Xi_Zhong_CV.pdf`
- Photo: replace `assets/img/prof_pic.jpg`

Every push to `main` automatically rebuilds and deploys the site.
