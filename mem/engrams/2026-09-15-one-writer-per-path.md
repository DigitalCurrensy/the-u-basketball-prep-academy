---
slug: one-writer-per-path
created: 2026-09-15
weight: 0.89
tags: [github, agents]
source: incident
---
# What happened
Multiple agents called create_or_update_file on the same hub paths. The tool can report success while main is missing the file. Rate limits (HTTP 429) made retries worse.

# Why it matters
One writer per path per session. Prefer one push_files commit for a file pack. Confirm with get_file_contents / raw main before retrying.

# Trigger
Any multi-agent GitHub write on DigitalCurrensy repos.
