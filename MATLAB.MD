# Implement and run MATLAB

Use the current task's inputs, not values copied from an old assessment. Prefer a single clearly named `.m` script that works when opened and run in MATLAB, with any required supporting files explicitly identified.

## Readable code

Use numbered `%%` sections, blank lines between logical stages, consistent indentation, and brief comments explaining purpose. Typical sections are setup, parameters, model, outcome classification, probabilities, expected value, verification, printed results, comparisons, and saved artifacts.

Keep comments natural and short. Explain a non-obvious decision rather than narrating every assignment statement. Preserve the calculations when a user requests only spacing or comments; verify that executable statements remain unchanged.

Use a recorded random seed and generator for reproducibility. Record the MATLAB version and parameters of the actual run. Version-dependent features should either be supported by the user's version or have a compatible alternative.

## Required output in the Command Window

Every value included in a report must be reproducible from the submitted script. Print clear labels, counts, probabilities, units, and expected value. Add space between result blocks.

If the document uses compact blocks for individual table rows, the same blocks must appear directly in the Command Window. Build them from calculated variables and print them, for example:

```matlab
fprintf('\nExpected value\n');
fprintf('Bet: PHP %.2f\n', bet);
fprintf('EV per game: PHP %.4f\n', expectedValue);
```

An image export or a message listing saved filenames does not satisfy a request to display the actual result in the terminal. If output formatting uses a helper, include that helper or integrate it into the final script. Do not leave a hidden dependency on a private task path.

## Execution and artifact handling

Run the exact final script in MATLAB when available, using background execution when desktop control was excluded. Do not describe Python or Octave output as a MATLAB run. Preserve existing user edits before making changes.

Save requested outputs relative to the script or a clearly defined task output directory. Do not hard-code the agent's personal path. Avoid unexpected pop-up figures; use hidden figures for background exports when appropriate. A request to see figures may require visible figures, within the user's access scope.

Do not delete unrelated files, close the user's live session, or install tools without the required authorization. Avoid `close all` or workspace-clearing commands when operating in a shared active session; isolated batch execution is preferable for a self-contained script.

Only export the evidence files needed for the task. When the user asks for terminal text, implement terminal text rather than adding extra exports. Existing files should not be described as newly generated unless verified.
