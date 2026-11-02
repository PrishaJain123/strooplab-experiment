# Limitations and reproducibility

## Limitations

- This is an educational and portfolio demonstration, not a validated clinical, diagnostic, or standalone research instrument.
- The main block balances condition counts (24 congruent and 24 incongruent), but individual word-ink pairings occur six times when matching and twice when nonmatching. Interpret the condition contrast as a comparison of these stimulus sets.
- Only four colors and four response keys are used. Keyboard layout, display, browser, and device performance can affect results.
- Browser timing is based on jsPsych performance timing, but the software does not control display hardware or guarantee laboratory-grade timing. A trial is flagged if its browser tab is hidden during the response; closing or refreshing the page still ends the session and does not provide recovery.
- The task runs without a backend. Results are not centrally collected, and researchers must receive participant exports through a separate process.
- Only mapped response keys are accepted; other keys are ignored, but an accidental press of a valid color key cannot be distinguished from an intended answer. The summary is descriptive. It does not compute confidence intervals, participant-level group statistics, exclusions beyond the documented rules, or statistical significance.

## Reproducibility checklist

1. Publish the exact project files and record the release or commit used for a data collection session.
2. Use the same browser/device setup where feasible and record relevant deviations.
3. Preserve original participant CSV files before combining or processing them.
4. Keep source filenames or a non-identifying session code so records can be traced to their source without embedding personal information in trial data.
5. Record the participant instructions, response mapping, timeout (3000 ms), and trial counts (10 practice, 48 main) alongside any analysis.
6. Report the balanced condition counts (24/24), the different repetition counts for matching and nonmatching pairings, and the documented accuracy and reaction-time inclusion rules.
7. Treat downloaded CSVs as sensitive if they contain identifying details; the page itself does not provide access controls or encryption for files saved or shared by users.
