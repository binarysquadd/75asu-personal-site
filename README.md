# Personal Website

Source for my personal website built with **Hugo**.

---

## Requirements

- Hugo

Install:
```bash
HUGO_VERSION=0.125.7

wget https://github.com/gohugoio/hugo/releases/download/v${HUGO_VERSION}/hugo_${HUGO_VERSION}_linux-amd64.deb
sudo dpkg -i hugo_${HUGO_VERSION}_linux-amd64.deb

rm hugo_${HUGO_VERSION}_linux-amd64.deb
hugo version
```


## Local Development

This repository uses a theme as a git submodule.

After cloning, you must initialize it:

```
git submodule update --init --recursive
```
If you skip this step, Hugo will fail with:
```
found no layout file for "html" for kind "home"
```
```
# Run with live reload:

hugo server --disableFastRender

# Open:

http://localhost:1313
```


## Build
```
# Generate static files:

hugo

# Output directory:

public/

# Do not edit files inside public/.
```

## Deployment

```
Cloudflare Pages
	•	Build command: hugo
	•	Output directory: public

Netlify
	•	Build command: hugo
	•	Publish directory: public

Vercel
	•	Framework: Other
	•	Build command: hugo
	•	Output directory: public
```


## Structure
```
content/    Markdown content
layouts/    Layout overrides
themes/     Hugo themes
public/     Generated site
config.yaml Site config
```

© 2025 Asutosh Panda
Built slowly. Maintained carefully.

