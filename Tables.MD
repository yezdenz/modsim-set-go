# Place results and code inside tables

Preserve the template's existing tables unless the user requests a structural change. The following layout is an editable default derived from this workflow. Apply only the parts authorized for the current task.

## Overall model table

Keep the existing prompt row. Put the overall simulation summary in its answer row. If the user asks for the model code below it, add a new full-width row immediately after that summary and insert the relevant model-code image.

The model excerpt should show the parameters, population or deck, random sampling, simulation loop, and state or hand-total calculation needed to understand the model. Use the actual current script, not an invented simplified version presented as its source.

## Four estimate rows

Keep the original left-hand question and right-hand result cell. Insert the corresponding MATLAB result in the right-hand cell. When requested, insert one new row immediately below each result row and merge it across the existing columns.

| Original result | Code image in the merged row below |
| --- | --- |
| Frequency of a special event | Event detection, event counts, and probability calculation |
| Player versus dealer wins | Outcome comparison, tie handling, and win probabilities |
| Expected player value | Net profit and expected-value calculation |
| Fairness and tie-rule effect | Tie detection, dealer allocation, and supporting probabilities or EV |

Do this for every requested row, not just the first example shown in a screenshot. Keep code images fully inside the merged cell. Show verified current line numbers if requested. Omitted ranges must be distinguishable from contiguous code; never renumber an excerpt as if it were the original script.

Do not add repeated `Code used...` labels, filenames, or decorative captions when the user has asked to remove them. Descriptive comments already present in the source may remain inside the code image.

## Explanation and numeric answer tables

Fill conceptual questions with natural explanations. Fill numeric answer rows with the actual MATLAB values and consistent precision, optionally showing count divided by trials. Do not add duplicate code to every repeated value unless requested.

For a question about increasing the sample size, a compact actual comparison output is useful supporting evidence. It does not replace the explanation, and it should not be added without scope for that extra evidence.

## Final expected-value table

Show the substituted formula, result per game, and interpretation. If the user asks for MATLAB evidence here as well, add a row beneath the computation containing the relevant code image and its actual output. A duplicate earlier EV section is not a reason to refuse this explicit request.

Keep the entire final EV section together where practical. Never mark a value as computed in MATLAB unless the submitted code computes it and a run supports it.
