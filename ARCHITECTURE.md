# Technical architecture

StroopLab is a static website with no server-side component. The HTML page bundles jsPsych and the task plugin; task flow, trial data, participant summaries, CSV generation, and researcher analysis all execute in the browser. GitHub Pages or another static host can serve the project files.

The landing page offers two views. The participant view runs practice and main trials, then shows a personal summary and CSV download. From the results screen, the completed session can be passed directly into the researcher view in page memory. The researcher view can also import local CSV files, calculates descriptive condition summaries, displays reaction-time distributions and trial rows, and exports a combined CSV. The views share the same page and styling, while imported researcher data is held only in page memory.

No network endpoint, account, database, or cross-participant storage is configured. A researcher who needs durable or centralized collection must separately choose and implement an appropriate consent, privacy, and storage process.
