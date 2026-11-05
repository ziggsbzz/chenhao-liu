# Chenhao Liu — Academic Homepage

刘宸昊（上海财经大学金融学院）个人学术主页，基于 Jekyll 静态站点，可部署至 Cloudflare Pages（国内访问友好）。

---

## 部署 Cloudflare Pages

1. 在 [Cloudflare Dashboard](https://dash.cloudflare.com/) → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**。
2. 选择 GitHub 仓库 **`ziggsbzz/chenhao-liu`**。
3. 构建设置（**Build configuration**）：

| 项 | 值 |
|---|---|
| **Production branch** | `main` |
| **Framework preset** | None |
| **Build command** | `gem install bundler && bundle install && bundle exec jekyll build` |
| **Build output directory** | `_site` |

4. **Environment variables**（可选）：`JEKYLL_ENV` = `production`
5. 保存并部署。首次构建约 1–3 分钟。

本地预览：

```bash
bundle install
bundle exec jekyll serve --livereload
```

---

## Deploy on Cloudflare Pages (English)

Static Jekyll site for **Chenhao Liu** (Assistant Professor, SUFE School of Finance). Layout inspired by clean academic homepages (e.g. [yiqingxu.org](https://yiqingxu.org/)).

**Connect this repo** in Cloudflare Pages with:

- **Production branch:** `main`
- **Build command:** `gem install bundler && bundle install && bundle exec jekyll build`
- **Build output directory:** `_site`
- **Framework preset:** None

Optional: set `JEKYLL_ENV=production`.

---

## Content

- Profile text and publications from `academic-profile.md` (no fabricated entries).
- Email: liuchenhao@sufe.edu.cn (no phone on site).
- SUFE faculty page: https://fin.sufe.edu.cn/Faculty/Resume/liu_chenhao
- **CV (PDF)** is a placeholder until a file is uploaded to the repo.

Edit `_data/publications.yml`, `_data/awards.yml`, and `_config.yml` to update the site.
