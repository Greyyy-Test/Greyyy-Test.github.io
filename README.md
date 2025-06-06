# LaMET Webpage

This is the official webpage of **Large Momentum Effective Theory (LaMET)**, a theoretical framework that allows the calculation of parton physics from lattice QCD using hadron states with large momenta.

The webpage is deployed at [https://lamet4parton.org/](https://lamet4parton.org/).

See [CONTRIBUTING.md](CONTRIBUTING.md) for how to contribute and submit pull requests.

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
    image: /assets/images/lamet.png
    image_alt: "Profile Photo"
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
   - There is also a template: `2024-06-06-post-template.md` in `_posts`.
2. Use the following front matter:

```yaml
---
title: "My Post Title"
date: 2024-06-06
layout: single
toc: true
toc_sticky: true
author_profile: false
sidebar:
  nav: "main"
categories:
  - blog
tags:
  - LaMET
---
```

Write your post content below the front matter.

---

## 🧩 Front Matter & Head Parameters (for Pages and Posts)

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

## 💡 Using Notices and Callouts

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

For more styles and details, see the [Minimal Mistakes Notices documentation](https://mmistakes.github.io/minimal-mistakes/post%20formats/post-notice/).

---

## 🚀 Preview the Website Locally

### Install Bundler

- **Windows**:
  ```bash
  gem install bundler
  ```
- **macOS** (with Homebrew):
  ```bash
  brew install ruby
  gem install bundler
  ```
- **Linux** (Debian/Ubuntu):
  ```bash
  sudo apt-get install ruby-full
  gem install bundler
  ```

### Start the Local Server

Go to the root directory of the repository and run the following commands:

```bash
# Install dependencies (first time only)
bundle install

# Start the local server
bundle exec jekyll serve
```

Then open http://localhost:4000 in your browser.

---

## 🎨 Adding a Favicon and App Icons

To add a favicon and app icons for your site:

1. Visit [RealFaviconGenerator](https://realfavicongenerator.net/) and upload your image to generate a full favicon package.
2. Download the generated files and place them in your site's root directory (or as instructed by the generator).

---

## 📚 More Information
- See `page_template.md` in `_pages` for a ready-to-copy template.
- See `2024-06-06-post-template.md` in `_posts` for a post template.
- Edit `_data/navigation.yml` to customize navigation menus.
- For more details, see the [Minimal Mistakes documentation](https://mmistakes.github.io/minimal-mistakes/docs/).

---

## 📜 Acknowledgements

This site is built with the [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes), © Michael Rose, distributed under the MIT License.


