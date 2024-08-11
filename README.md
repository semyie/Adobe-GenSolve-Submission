---

# 🖼️ Adobe GenSolve - Curve Detection, Regularization, and Occlusion Handling from CSV Files - Round 2 Submission

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Colab](https://img.shields.io/badge/Google-Colab-blue.svg)

This repository contains a Jupyter Notebook designed to detect, regularize, and enhance curves from a dataset of XY path coordinates stored in CSV files. The notebook processes the curves by identifying geometric shapes, detecting symmetry, handling occlusions, and completing incomplete curves. The results are then visualized and saved in multiple formats, including PNG, SVG, and CSV.

![Adobe GenSolve Round 2](https://github.com/user-attachments/assets/de3cee7f-c506-4119-ab32-4f9a106a058e)

## 🌟 Features

- **Curve Detection:** Identify geometric shapes (e.g., circles, rectangles) within the input data.
- **Regularization:** Automatically refine and regularize detected shapes for better accuracy.
- **Symmetry Detection:** Detect and apply symmetry to enhance the aesthetic of curves.
- **Occlusion Handling:** Identify and reconstruct curves that are partially occluded or missing sections.
- **Curve Completion:** Complete incomplete curves and ensure all paths are fully closed.
- **Multiple Output Formats:** Save the processed and regularized curves as CSV, PNG, and SVG files.
- **Visualization:** Display the regularized curves directly in the notebook as a PNG image.

## 🚀 How to Use

### Step 1: Clone the Repository

```bash
git clone https://github.com/semyie/Adobe-GenSolve-Submission
cd Notebook
```

### Step 2: Install Dependencies

Make sure you have the necessary libraries installed. You can install them using the following command:

```bash
pip install -r requirements.txt
```

### Step 3: Upload Your CSV File

Run the notebook in Jupyter or Google Colab. When prompted, upload your CSV file containing the XY path coordinates. The CSV file should have the following format:

```csv
path_id,segment_id,x,y
1,1,34.5,78.3
1,1,35.0,79.0
...
2,1,45.6,23.4
```

### Step 4: Execute the Code

Once the CSV file is uploaded, the code will process the paths and beautify the curves. It will:

1. **Regularize Shapes:** Identify shapes (like triangles, rectangles, circles) and regularize them.
2. **Detect Symmetry:** Find and apply symmetry where possible.
3. **Handle Occlusions:** Reconstruct curves that are partially occluded or missing sections.
4. **Complete Curves:** Ensure all curves are closed if necessary.
5. **Beautify Curves:** Final adjustments to enhance the curves' appearance.

### Step 5: View and Save the Results

The processed curves will be displayed in the notebook as a PNG image. Additionally, the following files will be saved:

- `beautified_curves.csv` - CSV file with the beautified XY coordinates.
- `output.png` - PNG image of the beautified curves.
- `output.svg` - SVG file of the beautified curves.

### Example:

```python
# Example usage:
image_path = "/content/output.png"
display_image(image_path)
```

This command will display the PNG image within the notebook.

## 📂 Output Formats

- **CSV:** `beautified_curves.csv` - The final XY coordinates after detection, regularization, and occlusion handling.
- **PNG:** `output.png` - A raster image of the beautified curves.
- **SVG:** `output.svg` - A vector image of the beautified curves.

## 📊 Dataset

The input data consists of XY path coordinates, formatted as described earlier. You can find a sample dataset [here](https://github.com/yourusername/dataset-link).

## 🎨 Example Outputs

Here’s an example of the beautified curves displayed as a PNG image:

![Output Example](output.png)

## 🛠️ Dependencies

- **Python 3.8+**
- **NumPy**
- **Matplotlib**
- **svgwrite**
- **OpenCV**
- **SciPy**

Install these dependencies via `pip`:

```bash
pip install numpy matplotlib svgwrite opencv-python-headless scipy
```

## 🤝 Contributing

Contributions are welcome! Please open an issue or submit a pull request.

---
