# Rao Shahzaib Blog

Personal DevOps blog of **Rao Shahzaib** — DevOps Engineer. Live at [blog.raoshahzaib.site](https://blog.raoshahzaib.site).

## What you'll find here

DevOps tutorials in **simple Roman Urdu**: Terraform, Kubernetes (K3s), AWS, Ansible and Proxmox labs and guides — written from practical experience, with working code examples and step-by-step guidance.

Featured series: **Container Networking From Scratch** — follow a packet's path through the Linux kernel, from network namespaces to NAT.

## Tech stack

- [Astro](https://astro.build) — static site generator
- Markdown content in `src/content/blog/`
- Deployed on Cloudflare Workers (see `wrangler.json`)

## Writing a new post

1. Add a markdown file in `src/content/blog/`, e.g. `my-new-post.md`
2. Include frontmatter:

```yaml
---
title: "Post title"
description: "Short SEO description (~150 chars)"
pubDate: "2025-09-26"
heroImage: "https://..."
tags: ["container-networking", "linux"]
---
```

3. Push to `main` — the site redeploys automatically.

## Links

- 🌐 Blog: https://blog.raoshahzaib.site
- 💻 GitHub: https://github.com/ShahzaibRao
- 🔗 LinkedIn: https://linkedin.com/in/rao-shahzaib
- 📧 Contact: contact@raoshahzaib.site
