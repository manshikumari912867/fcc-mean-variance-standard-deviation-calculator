# 📊 Mean-Variance-Standard Deviation Calculator
A Python data analysis application built for **freeCodeCamp's Data Analysis with Python Certification**. This project utilizes **NumPy** to transform 9-element numerical lists into 3x3 matrices and compute key statistical metrics along multiple axes.
---
## 🚀 Features & Calculations
The `calculate()` function accepts a list of 9 digits, converts it into a 3x3 NumPy matrix, and outputs a dictionary containing:
- **Mean**
- **Variance**
- **Standard Deviation**
- **Maximum**
- **Minimum**
- **Sum**
Calculations are evaluated along:
1. `Axis 0` (Columns)
2. `Axis 1` (Rows)
3. `Flattened` (Whole Matrix)
---
## 🛠️ Tech Stack & Requirements
- **Language:** Python 3
- **Library:** NumPy (`import numpy as np`)
---
## 💡 Example Usage & Output
```python
import mean_var_std
result = mean_var_std.calculate([0, 1, 2, 3, 4, 5, 6, 7, 8])
print(result)
Expected Return Format:
python


{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.6666666666666666, 0.6666666666666666, 0.6666666666666666], 6.666666666666667],
  'standard deviation': [[2.449489742783178, 2.449489742783178, 2.449489742783178], [0.816496580927726, 0.816496580927726, 0.816496580927726], 2.581988897471611],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
