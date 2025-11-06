# rockifanze.com

My personal website built with Hugo and hosted on GitHub Pages.

## About

This is a static website generated using [Hugo](https://gohugo.io/), a fast and flexible static site generator written in Go.

## Local Development

### Prerequisites

- [Go](https://golang.org/) (for installing Hugo)
- [Hugo](https://gohugo.io/)

### Installation

1. Install Hugo:
   ```bash
   go install github.com/gohugoio/hugo@latest
   ```

2. Clone this repository:
   ```bash
   git clone https://github.com/rockifanze/rockifanze.com.git
   cd rockifanze.com
   ```

3. Run the development server:
   ```bash
   hugo server
   ```

4. Visit `http://localhost:1313` in your browser

### Building

To build the static site:

```bash
hugo
```

The generated files will be in the `public/` directory.

## Deployment

This site is automatically deployed to GitHub Pages using GitHub Actions. When changes are pushed to the `main` branch, the workflow will:

1. Build the Hugo site
2. Deploy it to GitHub Pages

The site will be available at: https://rockifanze.github.io/rockifanze.com/

## Project Structure

```
.
├── .github/workflows/  # GitHub Actions workflows
├── archetypes/         # Content templates
├── content/            # Site content (Markdown files)
├── themes/simple/      # Custom Hugo theme
├── hugo.toml           # Hugo configuration
└── README.md           # This file
```

## Adding Content

Create a new post:

```bash
hugo new posts/my-new-post.md
```

Edit the created file in `content/posts/my-new-post.md` and set `draft: false` when ready to publish.

## License

This project is open source and available under the MIT License.
