---
name: knowledge-explorer
description: Explore a topic with rich media and structured knowledge cards.
---

# Knowledge Explorer

## Instructions
Call the run_js tool using scripts/index.html and a JSON string for data with these fields.

- query: required. Extract the main topic, entity, place, event, work, or concept.
- lang: required. Use the user's 2-letter language code.
- mode: required. One of overview, gallery, timeline, audio, compare, or study.
- related_queries: optional array used for comparison or related topics.
- include_images: required boolean.
- include_audio: required boolean.

## Behavior
- Prefer broad canonical topic names.
- Preserve specific years for recurring events when the user includes them.
- Keep the final response grounded in the tool result.
- If the tool returns a webview, briefly introduce what the user is seeing.
- If the exact answer is not available, say so plainly and provide the closest useful result.
- The final answer must be in the same language as the user's prompt.