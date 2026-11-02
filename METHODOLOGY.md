# Research methodology

## Task

StroopLab is a browser based color-word interference demonstration. On each trial, a participant identifies the ink color of a displayed color word with a keyboard response: R for red, G for green, B for blue, and Y for yellow. The instruction is to name the ink, not read the word.

## Blocks and stimuli

Participants complete 10 randomly generated practice trials with feedback, followed by 48 randomized main trials without feedback. Only the four mapped color keys are accepted during response trials; other keys are ignored. The main block has 24 congruent and 24 incongruent trials. Each matching word-ink pairing appears six times; each of the 12 nonmatching pairings appears twice. Each word and each ink color appears 12 times, and trial order is shuffled. A 500 ms fixation cross precedes each response stimulus. Practice feedback lasts 700 ms. Each response trial ends after a valid keypress or a 3000 ms timeout.

## Outcomes

Accuracy is the number of correct answered main trials divided by answered main trials, excluding trials flagged as interrupted. Omissions are timed-out response trials and are excluded from that accuracy denominator. If the browser tab is hidden during an active response trial, that trial is flagged as interrupted and excluded from accuracy and reaction-time estimates. Reaction-time summaries use correct main trials with positive numeric reaction times. The Stroop effect is the incongruent mean reaction time minus the congruent mean reaction time. It is descriptive and does not include an inferential statistical test.

## Randomization

The main-trial order is shuffled in the participant's browser on each run. No fixed random seed is used, so the exact sequence is not reproducible from the exported CSV alone. The CSV records the realized order and trial-level outcomes.
