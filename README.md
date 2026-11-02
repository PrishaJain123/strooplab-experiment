# StroopLab

A self-contained, browser-based Stroop color-word experiment with a participant results view and local researcher dashboard.

## Use

Open the site in a desktop browser. Choose **Participant view** to run 10 practice trials followed by 48 main trials (24 congruent and 24 incongruent), view personal results, and download a CSV. From the participant results screen, choose **Open researcher view with this session** to inspect and export that completed session directly in page memory. Choose **Researcher view · analyze CSV files** to load other participant CSVs locally, compare condition accuracy and reaction times, view distributions and trial records, and export a combined dataset.

## Privacy

No server or database is used. A session transferred to the researcher view remains in the current page only; CSV files selected for analysis are not uploaded. Participants and researchers are responsible for saving and sharing any downloaded exports.

## Documentation

- [Research methodology](METHODOLOGY.md)
- [Data processing](DATA-PROCESSING.md)
- [Technical architecture](ARCHITECTURE.md)
- [Limitations and reproducibility](LIMITATIONS-REPRODUCIBILITY.md)
- [Publishing instructions](PUBLISH.txt)

The bundled jsPsych software is distributed under the MIT License; see `jsPsych-license.txt`.
