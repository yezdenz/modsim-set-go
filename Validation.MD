# Verify the model and final artifacts

Choose checks that establish meaningful properties. Do not add a large test suite for a spacing-only change. Run the exact final script when code behavior changes and execution is available.

## Model and numerical checks

Check the population composition, valid state or total ranges, replacement rules, tie policy, and outcome accounting. Confirm that mutually exclusive complete outcomes sum to the number of trials and that probabilities are counts divided by the correct N.

Check expected value both from outcome counts and from the mean of the per-trial net-profit vector where practical. Verify the payout assumptions and units. An average per-game loss must not be confused with a total loss across the simulation.

Compare with a genuinely independent analytic argument or exact enumeration where practical. A calculation performed by AI is not proof of independent student verification. Record who or what performed each check.

Larger-N comparisons should disclose whether they are nested prefixes of one random stream or separate runs. Do not present a confidence interval as a guaranteed bound or random sample differences as proof of unfairness without reference to the model.

## Application execution

Verify the MATLAB version, seed, parameters, actual output, completion status, and any assertion results. Do not label an unexecuted script as tested. If MATLAB is unavailable, distinguish code preparation and alternative checks from the required MATLAB run.

Reproduce the exact compact blocks used in the report in the Command Window. Verify that the saved script contains any helpers necessary to generate them. Test from the expected run location so private hard-coded paths are not accidentally required.

## Document checks

Render every final page and inspect it visually. Confirm that the source template is preserved, answer text uses the intended local font, all images remain inside cells, code rows are actually merged, and source lines match the latest script.

Check that every requested table is filled, every original question remains, no removed caption has reappeared, and the final EV evidence is present if requested. Resolve blank trailing pages and orphaned headings through scoped layout fixes, without shrinking all content or changing unrelated formatting.

Reopen the actual saved files. Reconcile the document, code, logs, captures, plots, numeric results, and declaration. Apply [Submission.MD](Submission.MD) only after this final reconciliation.
