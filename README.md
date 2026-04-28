# LA_project_team18

Recovering images with missing pixels using Iterative SVD.

## Project Overview

This project demonstrates image recovery using singular value decomposition (SVD). A grayscale image is corrupted by removing a fraction of pixels, then recovered via:

- manual SVD reconstruction using eigen decomposition
- built-in NumPy SVD for comparison

The notebook includes visualization of the original image, corrupted image, and recovered results.

## Repository Structure

- `LA_project_Alania_Petrus_Trush.ipynb` - main Jupyter notebook with the full implementation
- `test.jpg` - example image used by the notebook
- `photos/` - additional image assets (optional)
- `README.md` - project documentation

## Requirements

- Python 3.9+ (recommended)
- Jupyter Notebook or JupyterLab
- Python packages:
  - `opencv-python`
  - `numpy`
  - `matplotlib`

## Setup Instructions

1. Open a terminal and change into the project folder:

```bash
cd /Users/lilialania/Documents/linear_algebra/project/LA_project_team18
```

2. Create and activate a virtual environment (recommended):

```bash
python3 -m venv venv
source venv/bin/activate
```

3. Install dependencies:

```bash
pip install opencv-python numpy matplotlib jupyter
```

## Running the Notebook

1. Start Jupyter Notebook or JupyterLab:

```bash
jupyter notebook
```

or

```bash
jupyter lab
```

2. Open `LA_project_Alania_Petrus_Trush.ipynb` in the browser.
3. Run the notebook cells in order.

## Usage Notes

- The notebook loads `test.jpg` from the project root.
- You can modify the following variables in the notebook to experiment:
  - `image_path` — image file path
  - `missing_rate` — fraction of pixels removed
  - `k` — number of singular values used for reconstruction
  - `iterations` — number of recovery iterations
  - `seed` — random seed for mask generation

## Expected Output

The notebook displays:

- original grayscale image
- corrupted image with missing pixels
- recovered image using manual SVD
- recovered image using built-in NumPy SVD
- the numerical difference between manual and built-in recovery

## Team Members

- Alania Lili
- Dominika Petrus
- Sofiia Trush

## References

This project is based on matrix completion and SVD techniques for image recovery.
