# Define the mathematical model

Translate the assessment into an explicit model before writing code. Record the trial, state, inputs, random draws, decision rules, outputs, and units. Keep the assumptions short enough for the student to explain.

## Sampling and outcomes

- Use the required finite population, distribution, or deck. Distinguish drawing with replacement from drawing without replacement.
- Preserve dependence within a trial. For a card game using one deck, dealing separate independently sampled hands may produce an incorrect model.
- State when the population resets between trials. A freshly shuffled deck per game differs from playing repeatedly through one shoe.
- Resolve equality, ties, exceptional outcomes, and ordering consistently. Every trial must have a defined outcome.
- Use the assigned number of trials for the main answers. Extra runs are comparisons, not replacements for the required run.

## Probabilities and expected value

Estimate each event probability as its count divided by the number of trials. Distinguish overlapping events from mutually exclusive outcomes. Two participants can both have the same special hand; adding their individual event probabilities may double-count trials.

For an even-payout win/loss model with no pushes:

```matlab
expectedValue = bet * (playerWins - dealerWins) / N;
```

Here `playerWins` and `dealerWins` are counts. With probabilities instead, omit the division by `N`. Define profit as net profit, not total payout including the returned stake. Include pushes, fees, unequal payouts, or variable stakes when the actual rules require them.

State the currency and whether the result is per game or across all games. A negative player EV favors the house under the defined model. Zero is a fair expected return, not evidence that the player has an advantage. Do not rewrite source wording to hide such a distinction; explain it in the answer.

## Comparison and interpretation

Use analytic calculations or exact enumeration where practical. They must match the same finite population, rules, and payout assumptions. Do not call an additional simulation an exact calculation.

For independent trials, sampling uncertainty generally decreases on the order of `1/sqrt(N)`. Estimates need not improve monotonically on each increase. Larger samples reduce random variation; they do not eliminate a biased game rule.

Explain why the result follows from the model. Keep a model limitation distinct from a coding error or a random fluctuation.
