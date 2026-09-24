# Publishing the root site

This folder retains its existing Git history and master branch.

Publish this repository to GitHub under the owner the-other-hello-there with the repository name the-other-hello-there.github.io. The local folder name GithubMainRepo is fine.

In GitHub Pages settings, select Deploy from a branch and the branch containing these files (currently master), with / (root) as the folder.

After deployment, verify:
- https://the-other-hello-there.github.io/robots.txt displays the crawler rules as plain text.
- https://the-other-hello-there.github.io/ redirects to /HenryLuo-Portfolio/.

No remote was configured when these files were added. If connecting to an existing GitHub repository, first fetch and inspect its history. If it has a different initial commit, clone that repository and copy these site files into the clone rather than force-pushing or copying a .git directory.

## Updating the rules

The source of truth remains ../HenryLuo-Portfolio/scripts/search-selection.json. From the portfolio folder, run:

```powershell
python scripts/build_search.py
python scripts/build_search.py --check
```

Then from GithubMainRepo:

```powershell
Copy-Item -LiteralPath ../HenryLuo-Portfolio/robots.txt -Destination ./robots.txt
git diff -- robots.txt
```

Review, commit, and push using your normal Git workflow. Keep sitemap.xml in the HenryLuo-Portfolio repository. Only the generated robots.txt needs to be copied here after policy changes.