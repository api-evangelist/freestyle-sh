---
title: "The Best Way to Move Local Files Into a Sandbox"
url: "https://www.freestyle.sh/blog/product/best-way-move-local-files-to-sandbox"
date: "2026-06-06"
author: "Freestyle Team"
feed_url: "https://www.freestyle.sh/blog"
---
File transfer into sandboxes is one of the first architecture decisions in an agent product, with different situations calling for different solutions — Git is best when the sandbox should preserve history, branches, diffs, and review, while scp is best when a human needs to push a small thing quickly. Upload files to sandbox encompasses multiple distinct workflows rather than a single feature, and the right solution depends on the shape of the work.
