# Site template for Hexo Next

- [Hexo](https://hexo.io/zh-tw/) static site generator.
- Fast and elegant [Next theme](https://theme-next.js.org/).
- GitHub actions and GitLab CI enabled to build the websites to [GitHub pages](https://pages.github.com/) and [GitLab pages](https://docs.gitlab.com/ee/user/project/pages/).

## Copy over my template site

- Hosting GitHub: click `use as template`
- Hosting on others e.g. GitLab: clone / import this repo

In `_config.yml`, Change `baseurl` and your personal settings. See also [Hexo configuration](https://hexo.io/docs/configuration.html).
```yml _config.yml
url: https://username.github.io
root: /repo-name/  # root:/ for personal website (username.github.io)
```

### Notes On GitHub

Open your repository settings => Pages => GitHub Pages
=> Build and deployment => Source, Select `GitHub actions`


In `_config.next.yml`, change the settings of the Next theme. See also [Next theme settings](https://theme-next.js.org/docs/theme-settings/).

## Livereload

Use the `browse-sync` proxy.

```bash
npm install -g browser-sync
```

And the in the project folder
```bash
browser-sync start --proxy localhost:4000 --files *
```
