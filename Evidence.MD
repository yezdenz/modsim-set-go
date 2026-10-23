# Maintain a private evidence register

Create one register per assessment in the private task workspace. Do not commit its completed contents to this workflow repository.

Use this structure:

| Requirement | Source location | Implementation | Actual run and parameters | Evidence type and file | Final document location | Status |
| --- | --- | --- | --- | --- | --- | --- |
| Required result | Page, table, or question | Script section or lines | Application/version, seed, N, settings | Capture, log, image, or calculation | Table and row or verified page | Pending / prepared / executed / reviewed |

Keep the stages distinct. Writing code is preparation. Inspecting syntax is a source check. Running the target program is execution. Reviewing its output and placement is evidence review. A successful document render does not establish that the model ran correctly.

Record model assumptions, output units, probability precision, and whether a displayed value is estimated or exact. Map the calculation, printed block, result image, prose, and final table to the same underlying run.

For code images, record the current script path and actual line ranges. For rendered captures, retain their source log or data. For screenshots, record the actual application and permitted capture method. Do not use a generated image to conceal missing execution.

When the code or parameters change, invalidate dependent evidence until reconciled. Regenerate only the affected outputs, then inspect the updated document. Do not keep an old plot, stale line number, or contradictory expected-value explanation merely because the file still exists.

Record unsupported claims, classification conflicts, missing access, and student-only steps as pending. Do not convert them into checked items or an unqualified ready status.
