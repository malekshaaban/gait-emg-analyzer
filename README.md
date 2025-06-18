Gait and EMG Signals Analyzer
This MATLAB application analyzes gait patterns and electromyography (EMG) signals, designed to process and visualize data for biomechanical research. It includes functionality for loading MVNX motion capture data, filtering EMG signals, and plotting gait cycles with options to highlight variability.
Files

Gait_And_Emg_Signals_Analyzer.mlapp: The main MATLAB App Designer application providing a user interface for gait and EMG analysis.
load_mvnx.m: A MATLAB script for loading and processing MVNX (motion capture) data files.
LOGO2.png: The application logo displayed in the user interface.

Features

Data Loading: Import MVNX files for gait data using load_mvnx.m.
EMG Processing: Filter and segment EMG signals for analysis, with robust handling of noisy data.
Visualization: Plot individual gait cycles as lines and overlay multiple cycles as shaded areas to show variability (e.g., across 89 cycles).
Customizable Display: Option to plot EMG data on the same axis as gait cycles or on a separate axis, configurable via a settings checkbox in the app.

Requirements

MATLAB: Version R2019b or later.
Toolboxes: Signal Processing Toolbox (optional for advanced filtering; basic filtering works without it).
Dependencies: No external libraries required beyond MATLAB. Ensure MVNX files are compatible with the load_mvnx.m script.

Installation

Clone the repository:git clone https://github.com/malekshaaban/gait-emg-analyzer.git


Open MATLAB and navigate to the project folder:cd 'path/to/gait-emg-analyzer'


Open Gait_And_Emg_Signals_Analyzer.mlapp in MATLAB App Designer.

Usage

Launch the app by double-clicking Gait_And_Emg_Signals_Analyzer.mlapp in MATLAB or running it from the App Designer.
Use the app’s interface to load MVNX data via load_mvnx.m.
Configure settings (e.g., select whether to plot EMG data on the same or separate axes).
Analyze gait cycles and EMG signals, with options to visualize variability and validate results.


Notes

Data Privacy: Ensure MVNX and EMG data files do not contain sensitive information before sharing.
Performance: For large datasets, processing time may vary. Optimize by limiting the number of cycles plotted.
Compatibility: The app avoids using nanmean and nanstd to ensure compatibility without the Statistics Toolbox, using base MATLAB functions with manual NaN handling.


Contributing
Contributions are welcome! Please submit a pull request or open an issue on GitHub for suggestions or bug reports.
Contact
For questions or support, contact malekshaaban.
