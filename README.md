# LaMET Webpage

This is the official webpage of **Large Momentum Effective Theory (LaMET)**.

---

## 📄 Adding a New Page

To add a new page:
1. Copy the template file: `page_template.md` from the `_pages` directory.
2. Rename it (e.g., `my-new-page.md`) and edit the content as needed.
3. Place your new file in the `_pages` directory.
4. Add a navigation entry in `_data/navigation.yml` if you want it to appear in the sidebar or top menu.

**Example front matter for a new page:**
```yaml
---
title: "My New Page"
permalink: /my-new-page/
layout: single
toc: true           # Show table of contents (right sidebar)
toc_sticky: true    # Make TOC sticky while scrolling
sidebar:
  - title: "Welcome"
    text: "This is a custom sidebar block."
---
```

- `toc`: Show the "On this page" table of contents (right sidebar, auto-generated from headings)
- `toc_sticky`: Make the TOC sticky (remains visible while scrolling)
- `sidebar`: Custom left sidebar content (see Minimal Mistakes docs for more options)

For more advanced sidebar navigation, you can use:
```yaml
sidebar:
  nav: "main"  # or "docs", as defined in _data/navigation.yml
```

---

## 📝 Adding a New Post

To add a new blog post:
1. Create a new file in the `_posts` directory, named as `YYYY-MM-DD-title.md` (e.g., `2024-06-06-my-post.md`).
2. Use the following front matter:

```yaml
---
title: "My Post Title"
date: 2024-06-06
layout: single
toc: true
---
```

Write your post content below the front matter.

---

## 🧩 Page Head Parameters Explained

- `title`: The page or post title (displayed at the top and in navigation)
- `permalink`: The URL path for the page (e.g., `/about/`)
- `layout`: Page layout, usually `single` for documentation or posts
- `toc`: Show the right-side table of contents (auto-generated from headings)
- `toc_sticky`: Make the TOC sticky while scrolling
- `sidebar`: Custom left sidebar content or navigation menu
    - Use a list of blocks for custom content (see above)
    - Or use `nav: "main"` to use a navigation group from `_data/navigation.yml`
- `author_profile`: Show or hide the author profile in the sidebar (`true`/`false`)
- `last_modified_at`: (Optional) Last updated date for the page

---

## 📚 More Information
- See `page_template.md` in `_pages` for a ready-to-copy template.
- Edit `_data/navigation.yml` to customize navigation menus.
- For more details, see the [Minimal Mistakes documentation](https://mmistakes.github.io/minimal-mistakes/docs/).

---

## Using Notices and Callouts

You can use special callout blocks to highlight information in your Markdown files. For example:

```markdown
This is an info notice.
{: .notice--info}

This is a success notice.
{: .notice--success}

This is a warning notice.
{: .notice--warning}

This is a primary notice.
{: .notice--primary}
```

For more styles and details, see the [Minimal Mistakes Notices documentation](https://mmistakes.github.io/minimal-mistakes/docs/helpers/#notices).

---

## Troubleshooting

If you have a question about using Jekyll, start a discussion on the [Jekyll Forum](https://talk.jekyllrb.com/) or [StackOverflow](https://stackoverflow.com/questions/tagged/jekyll). Other resources:

- [Ruby 101](https://jekyllrb.com/docs/ruby-101/)
- [Setting up a Jekyll site with GitHub Pages](https://jekyllrb.com/docs/github-pages/)
- [Configuring GitHub Metadata](https://github.com/jekyll/github-metadata/blob/master/docs/configuration.md#configuration) to work properly when developing locally and avoid `No GitHub API authentication could be found. Some fields may be missing or have incorrect data.` warnings.

---

## Acknowledgements

This site is built with the [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes), © Michael Rose, distributed under the MIT License.

---

## Adding a Favicon and App Icons

To add a favicon and app icons for your site:

1. Visit [RealFaviconGenerator](https://realfavicongenerator.net/) and upload your image to generate a full favicon package.
2. Download the generated files and place them in your site's root directory (or as instructed by the generator).
