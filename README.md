# My Personal Website

This is my personal website built using [Hugo](https://gohugo.io/) and the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme. It serves as a platform for sharing my thoughts, experiences, and adventures.

## Features

- Clean, responsive design using PaperMod theme
- Custom font styling using Lato
- Blog posts with reading time
- Table of contents for longer posts
- Social media integration
- Dark/Light mode support

## Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (latest version recommended)
- Git

## Local Development

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd site
   ```

2. Initialize and update the theme submodule:
   ```bash
   git submodule init
   git submodule update
   ```

3. Start the Hugo development server:
   ```bash
   hugo server -D
   ```

4. Visit http://localhost:1313 to see the site

## Creating Content

### New Blog Post
```bash
hugo new posts/my-post-name.md
```

### Adding Images
1. Place images in the `static/images` directory
2. Reference in markdown: `![Alt text](/images/image-name.jpg)`

## Building for Production

To build the site for production:
```bash
hugo --minify
```

This will create an optimized build in the `public` directory.

## Customization

- Site configuration: Edit `config.toml`
- Custom styling: Edit `assets/css/extended/custom.css`
- Content: Add/edit files in the `content` directory

## Deployment

The site is configured for production with:
- Minified assets
- Optimized images
- Production environment settings

## License

This project is licensed under the MIT License - see the LICENSE file for details. 