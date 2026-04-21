# COMP3516 Group Project

This repository contains our COMP3516 group project on multi-modal human activity recognition using the OctoNet dataset.

## Project Structure

- `instructions.ipynb`: Main notebook containing Task 1, Task 2, and Task 3 code.
- `data_sources/`: Local dataset folder containing the `.pickle` sample files. This folder is required to run the notebook but is ignored by git.
- `activity_masked.csv`: Input CSV with masked labels used for prediction.
- `activity_ira.csv`: Prediction output for the IRA-only model.
- `activity_wifi.csv`: Prediction output for the WiFi-only model.
- `activity_imu.csv`: Prediction output for the IMU-only model.
- `activity_multi.csv`: Prediction output for the multimodal model.
- `output_visualizations/`: Saved figures and trained model checkpoints.
- `latex_template/`: LaTeX files for the final report.

## Setup

1. Clone the repository.
2. Place the dataset folder inside the project root so the path is `data_sources/`.
3. Make sure Python and the required libraries are installed.

Recommended libraries:
- `numpy`
- `matplotlib`
- `torch`
- `pickle` (standard library)
- `csv` (standard library)
- `pathlib` (standard library)

## Running the Project

1. Open `instructions.ipynb` in Jupyter Notebook or VS Code.
2. Run the notebook cells in order.
3. Task 1 generates visualization images.
4. Task 2 trains single-modality models and exports the prediction CSV files.
5. Task 3 trains the multimodal model and exports `activity_multi.csv`.

## Reproducibility Notes

- The notebook sets a fixed random seed for reproducibility.
- Trained checkpoints are saved in `output_visualizations/`.
- CSV outputs follow the format required by the assignment.

## Submission Files

The final submission should include:
- all code
- trained checkpoints
- `activity_ira.csv`
- `activity_wifi.csv`
- `activity_imu.csv`
- `activity_multi.csv`
- the final report PDF generated from `latex_template/`

## Notes

- `data_sources/` is not committed to GitHub because it is large and intended to stay local.
- Run the notebook from the project root so relative paths resolve correctly.
