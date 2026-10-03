# Pausetide website

This folder is a self-contained static website for GitHub Pages. It uses plain HTML and CSS with no JavaScript, analytics, cookies, external fonts, or trackers.

## Before publishing

Open `index.html` locally in a browser and check all three pages and links.

## Publish with GitHub Pages

From the repository root, commit the `website/` folder to your normal branch. Then publish only this folder to a Pages branch:

```sh
git subtree split --prefix website -b pausetide-pages
git push origin pausetide-pages:gh-pages --force
git branch -D pausetide-pages
```

In GitHub:

1. Open the repository.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select the `gh-pages` branch and the `/(root)` folder.
5. Select **Save**.

GitHub will show the published URL after deployment. For a standard project repository it will usually be:

```text
https://<YOUR_GITHUB_USERNAME>.github.io/<REPOSITORY>/
```

The policy and support URLs will be:

```text
https://<YOUR_GITHUB_USERNAME>.github.io/<REPOSITORY>/privacy.html
https://<YOUR_GITHUB_USERNAME>.github.io/<REPOSITORY>/support.html
```

To publish a later update, run the same three commands again after committing the changes.
