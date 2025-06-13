# MoBI Lab Software

This page contains information and links to relevant software developed by the CMI MoBI Core in support of MoBI Lab infrastructure.

**MoBI View** ([https://github.com/childmindresearch/MoBI-View](https://github.com/childmindresearch/MoBI-View)) combines all incoming MoBI data streams into one synchronized interface with real-time feedback.

**MoBI Quality** ([https://github.com/childmindresearch/MOBI_QC](https://github.com/childmindresearch/MOBI_QC)) performs basic preprocessing and quality control metrics into a PDF report for a variety of MoBI data types.

**MoBI Protocol** ([https://github.com/childmindresearch/graphomotor_cmi](https://github.com/childmindresearch/graphomotor_cmi)) is the current data collection protocol for MoBI-Graphomotor tasks.

**MoBI Motion** software works with motion tracking data from the Zed 2i depth camera system. Zed2i 3D Capture ([https://github.com/childmindresearch/zed2i_3d_capture](https://github.com/childmindresearch/zed2i_3d_capture)) enables standalone data collection; Zed2i 3D LSL Capture ([https://github.com/childmindresearch/zed2i_3d_lsl_capture](https://github.com/childmindresearch/zed2i_3d_lsl_capture)) enables multimodal data collection; MoBI Motion Tracking ([https://github.com/childmindresearch/mobi-motion-tracking](https://github.com/childmindresearch/mobi-motion-tracking)) provides data analysis and scoring methods; and Zed2i Motion Classifier ([https://github.com/childmindresearch/zed2i_motion_classifier](https://github.com/childmindresearch/zed2i_motion_classifier)) performs real time action, behavior, and position classifications for use in quality control analysis.

**MoBI Graphomotor** ([https://childmindresearch.github.io/graphomotor/graphomotor.html](https://childmindresearch.github.io/graphomotor/graphomotor.html)) enables preprocessing, feature extraction, and visualization of the results Curious-based ([https://www.gettingcurious.com/](https://www.gettingcurious.com/)) graphomotor tasks, like Archimedean Spiral Tracing, Rey-O Complex Figure Drawing, Alphabet Writing, Symbol Digit Substitution, and Trails tasks.

**MoBI AV** ([https://github.com/childmindresearch/MoBI-AV](https://github.com/childmindresearch/MoBI-AV)) connects to microphone and camera hardware and acquires high-bandwidth audio and video data in real-time for temporal synchronization with other MoBI data streams.

**MoBI Impedance** ([https://github.com/childmindresearch/MoBI_dry_eeg_lsl](https://github.com/childmindresearch/MoBI_dry_eeg_lsl)), based on work from Wearable Sensing, allows for simultaneous measurement of both EEG signals and electrode impedances.

**MoBI SceneCam** (Link coming soon!) connects to the Pupil Labs Neon eye tracking system to enable time synchronized capture of scene camera video data.

**MoBI Electrophysiology** (Link coming soon!) connects to the Plux Biosignals electrophysiology hub and rectifies Bluetooth connection issues commonly encountered with the Open Signals software.

**SenseLab** ([https://github.com/sensein/senselab](https://github.com/sensein/senselab)), developed by the SenseIn group with the support of the Child Mind Institute's MoBI Core, streamlines the processing and analysis of behavioral data, such as voice and speech patterns, with robust and reproducible methodologies.

**MoBI Actigraphy** works with wrist worn accelerometer data to investigate sleep and activity patterns outside the lab. Wristpy ([https://childmindresearch.github.io/wristpy/wristpy.html](https://childmindresearch.github.io/wristpy/wristpy.html)) processes and analyzes data from GENEActiv and Actigraph devices. Wristpy Post Proc ([https://github.com/childmindresearch/wristpy_post_proc](https://github.com/childmindresearch/wristpy_post_proc)) provides a set of pipeline and utilities to compute key metrics about sleep from already processed wrist-worn actigraphy data. ActiSleep Tracker ([https://github.com/childmindresearch/actisleep-tracker](https://github.com/childmindresearch/actisleep-tracker)) allows for manual editing and annotation of sleep data.

**Lab Streaming Layer** ([https://labstreaminglayer.org/](https://labstreaminglayer.org/)) underpins all the above software.