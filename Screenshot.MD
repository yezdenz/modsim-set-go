# Images and evidence provenance

Choose the evidence type that the assignment and user actually require. Record the type privately and describe it accurately.

| Type | Meaning | What it can establish |
| --- | --- | --- |
| Interface screenshot | Capture of the actual MATLAB editor, Command Window, or figure window | The visible application state and output at capture time |
| MATLAB output capture | Text or data from an observed MATLAB run rendered into an image | The recorded output, with its execution log as provenance |
| Code image | Rendered excerpt of the actual source file, optionally with line numbers | The source text and its mapping to the script |
| Illustration | A diagram or explanatory mockup | An explanation only; not execution evidence |

A rendered capture is not a literal screenshot of the MATLAB interface. Do not claim that they look identical. Font, theme, cropping, and arrangement can differ while the code and numeric values remain the same. If the rubric specifically requires interface screenshots, rendered captures do not fulfill that requirement without accepted permission to substitute them.

## Capture without disturbing the user

Reuse user-supplied screenshots or use a permitted isolated capture method. Do not take over the desktop merely because images are required. If literal interface captures need user participation, identify the exact view needed and keep that evidence item pending.

Never fabricate editor chrome, terminal output, success messages, timestamps, or code line numbers. Do not use generative image tools to create factual code or result evidence.

## Readability and consistency

Prefer a light background for generated code and output images when the user requests it. Preserve the factual text and values. For genuine screenshots, keep the original capture and any permitted cropped or redacted derivative distinguishable; do not recolor a capture and call it untouched.

Keep code text legible at its inserted size. Preserve aspect ratio. Add enough whitespace to avoid clipping or masking cell borders. Use the table's actual usable width, not a guessed page width. Retain image data inside the DOCX.

When showing selected source lines, extract them from the current script. Recheck line numbers after any code edits. A picture prepared before a code change may be stale even if it looks correct.

Keep raw run logs and source hashes privately where useful. Never include unrelated windows, credentials, unnecessary personal details, or private reference material in public workflow files.
