---
name: knowledge-explorer
description: Query summary information from Wikipedia for a given topic.
---

# Knowledge Explorer

## Instructions

Call the `run_js` tool with the following exact parameters:
- script name: index.html
- data: A JSON string with the following fields:
  - query: String. The topic to search for.
  - lang: String. The two-letter language code.

## Behavior
- Extract the main topic from the user's request.
- Use the user's language when possible.
- Keep your final response grounded in the tool result.