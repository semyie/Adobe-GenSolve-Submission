Here is a sample GitHub README file that explains how to use the provided notebook, includes instructions for users to input their own CSV files, and details the output formats.

---

# 🖼️ Beautify and Visualize Curves from CSV Files

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Colab](https://img.shields.io/badge/Google-Colab-blue.svg)

This repository provides a Jupyter Notebook that takes in a CSV file containing XY path coordinates, processes the curves by detecting symmetry, completing incomplete curves, and beautifying them. The results are then visualized and saved in multiple formats including PNG, SVG, and CSV.

## 🌟 Features

- **CSV Input:** Easily upload your CSV file containing XY coordinates using a file selection button.
- **Curve Beautification:** Automatically regularizes shapes, detects symmetry, and completes curves.
- **Multiple Output Formats:** Save the processed curves as CSV, PNG, and SVG files.
- **Visualization:** Display the beautified curves directly in the notebook as a PNG image.

## 🚀 How to Use

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/Beautify-Curves.git
cd Beautify-Curves
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
3. **Complete Curves:** Ensure all curves are closed if necessary.
4. **Beautify Curves:** Final adjustments to enhance the curves' appearance.

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

- **CSV:** `beautified_curves.csv` - The final XY coordinates.
- **PNG:** `output.png` - A raster image of the beautified curves.
- **SVG:** `output.svg` - A vector image of the beautified curves.

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

This README file provides clear instructions for using the notebook, making it easy for users to input their own files and view the results. It also uses emojis, badges, and visual elements to make the content more engaging.
