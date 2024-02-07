# GNSS

## Overview
This repository contains code for GNSS (Global Navigation Satellite System) positioning using pseudorange measurements from smartphone sensor data. The code is designed to process GNSS data collected during vehicle trips and estimate the position of the smartphone along with velocity using robust weighted least squares (WLS) and Kalman filtering techniques.

## Contents
- **gnss_positioning.ipynb**: Jupyter notebook containing Python code for GNSS positioning.
- **README.md**: This README file providing an overview of the project.
- **data**: Directory containing sample GNSS data for testing the code.
- **requirements.txt**: Text file listing the required Python libraries and their versions.

## Usage
1. **Clone the Repository**: Clone this repository to your local machine using the following command:
   ```
   git clone Google smartphone decimeter challenge 2023/google-smartphone-decimeter-challenge-2023.git
   ```

2. **Install Dependencies**: Install the required Python dependencies by running:
   ```
   pip install -r requirements.txt
   ```

3. **Run the Code**: Open and run the `gnss_positioning.ipynb` Jupyter notebook to execute the GNSS positioning code. Make sure to provide the appropriate paths to your GNSS data files.

4. **View Results**: After running the code, you can view the results such as position estimates, velocity estimates, distance errors, and speed errors in the notebook.

## Data
The `data` directory contains sample GNSS data for testing the code. You can replace these sample files with your own GNSS data files for analysis.

## Requirements
The code is developed using Python 3 and requires the following libraries:
- `numpy`
- `pandas`
- `seaborn`
- `matplotlib`
- `scipy`
- `tqdm`
- `pymap3d`
- `geopy`

You can install these dependencies using the provided `requirements.txt` file.

## Author
- **Your Name**: [Your GitHub Profile](https://github.com/awrsha)

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- This project is based on the research and work of [original author's name] and their paper titled [paper title]. We acknowledge their contributions to the field of GNSS positioning.
- We thank the contributors to the open-source libraries used in this project for their valuable work.
- Special thanks to [anyone you want to acknowledge for their assistance or support].
