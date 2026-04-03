---
name: knowledge-explorer
description: Explore a topic with Wikipedia summaries, Wikimedia images, and structured knowledge cards.
---

# Knowledge Explorer

## Instructions

Call the `run_js` tool with the following exact parameters:
- script name: index.html
- data: A JSON string with the following fields:
  - query: String. The main topic, entity, place, event, work, or concept.
  - lang: String. The 2-letter language code matching the user's language.
  - mode: String. One of `overview`, `gallery`, `timeline`, `audio`, `compare`, or `study`.
  - related_queries: Array of strings. Optional. Used for comparison or related topics.
  - include_images: Boolean. True when images would help.
  - include_audio: Boolean. True when the user asks for audio, pronunciation, or spoken-style output.

## Behavior
- Prefer broad canonical topic names.
- Preserve specific years for recurring events when the user includes them.
- Use `gallery` mode when the user asks for images or visual exploration.
- Use `compare` mode only when the user clearly wants multiple topics contrasted.
- Keep the final response grounded in the tool result.
- If the tool returns a webview, briefly introduce what the user is seeing.
- If the exact answer is not available, say so plainly and provide the closest useful result.
- The final answer must be in the same language as the user's prompt.