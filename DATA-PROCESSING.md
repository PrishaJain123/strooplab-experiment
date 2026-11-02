# Data processing

## Participant export

The participant CSV contains one row per practice or main response trial. It includes trial number, phase, word, ink color, condition, key pressed, correctness, timeout status, interruption status, and reaction time in milliseconds. A timed-out trial has an empty response and reaction time, `Correct=FALSE`, and `Timed Out=TRUE`. `Interrupted=TRUE` means the browser tab became hidden during that response trial. Other non-response plugin trials (fixation and feedback) are not included in the export.

## Researcher import

The researcher dashboard accepts one or more CSV files and reads them locally in the browser. It recognizes the StroopLab column names case-insensitively, ignores practice rows when a Phase column is present, and analyzes rows whose condition is `congruent` or `incongruent`. If a Phase column is absent, matching condition rows are treated as analysis rows. Source filenames are retained to distinguish uploaded sessions. When the participant results screen opens the researcher view, that session is added from jsPsych data in memory with the source label `Current participant session`.

## Summary rules

- Condition accuracy: correct / answered, non-interrupted trials for that condition.
- Omissions: rows flagged `Timed Out=TRUE` (or legacy rows with no response and no correctness value).
- Mean and median reaction time: correct, non-interrupted trials with positive numeric RT, separately by condition.
- Stroop effect: incongruent mean RT minus congruent mean RT; shown as unavailable if either condition has no valid RT.
- Reaction-time histograms: eight shared-width bins based on the maximum valid RT in the loaded dataset.

The combined CSV export contains normalized main-task rows plus source filename. Imported files are not uploaded, saved to a server, or retained after the page is closed. Omission and interruption counts can overlap when a timed-out response trial was also interrupted. The dashboard does not impute missing responses or reaction times.
