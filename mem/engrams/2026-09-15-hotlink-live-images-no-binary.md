---
slug: hotlink-live-images-no-binary
created: 2026-09-15
weight: 0.90
tags: [docs, github, assets]
source: incident
---
# What happened
User asked for screenshots of the platform. GitHub MCP cannot push binary images. Live files already exist under /assets/img/.

# Why it matters
Hotlink https://www.theubasketballprepacademy.com/assets/img/{file}. Keep the same filename on the website and the README updates itself. Captions must match live alt text. Do not commit screenshot binaries to this hub.

# Trigger
README screenshots, social preview, or any request to "add photos to the repo."
