---
name: knowledge-explorer
description: Get a short Wikipedia summary for a topic, optionally with one image.
---

# Knowledge Explorer

## Instructions

Call the `run_js` tool with these exact parameters:
- script name: index.html
- data: A JSON string with:
  - query: String
  - lang: String
  - include_images: Boolean

Use this skill when the user asks about a topic, person, place, event, or concept.
Keep the final answer short and grounded in the tool result.