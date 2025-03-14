# My Adventure Blog

This is a Hugo-based personal blog for documenting treks, adventures, and sharing photos.

## Setup

1. Install Hugo (Extended version) following the [official guide](https://gohugo.io/installation/)
2. Clone the PaperMod theme:
   ```bash
   git clone https://github.com/adityatelange/hugo-PaperMod themes/PaperMod
   ```
3. Start the Hugo server:
   ```bash
   hugo server -D
   ```
4. Visit http://localhost:1313 to see your site

## Adding Content

### Create a new blog post
```bash
hugo new posts/my-first-post.md
```

### Create a new trek post
```bash
hugo new treks/my-first-trek.md
```

### Add images
1. Place images in the `static/images` directory
2. Reference them in your posts using: `/images/your-image.jpg`

## Deployment
Build the site using:
```bash
hugo
```
The static files will be generated in the `public` directory. 