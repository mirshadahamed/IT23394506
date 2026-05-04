# IT23394506
# 🧪 Playwright Automation Test – PixelsSuite
# ITPM Assignment 1 - Option 1 (IT23364506)

## 📌 Project Overview

This project automates the testing of the **preview functionality** of the PNG conversion feature on the PixelsSuite website.

The automation script uploads a PNG image, verifies whether the preview is displayed correctly, captures a screenshot, and records the results in a CSV file.

---

## 🌐 Website Tested

* https://www.pixelssuite.com/convert-to-png

---

## 🎯 Objective

To verify that:

* A PNG image can be uploaded successfully
* The preview section is displayed after upload
* The system behaves correctly under normal conditions

---

## 🛠️ Technologies Used

* Python 3.11 / 3.12
* Playwright
* openpyxl (for Excel handling)

---

## 📂 Project Structure

```
test_automation_ui/
│
├── image_preview_test.py       # Automation script
├── execution_results.csv       # Test results
├── sample.png                  # Test image (auto-created if missing)
├── results/
│   └── preview_pass.png        # Screenshot of result
└── README.md                   # Project documentation
```

---

## ⚙️ Setup Instructions

### 1. Install Dependencies

Run the following commands:

```
python -m pip install --upgrade pip
python -m pip install playwright openpyxl
python -m playwright install
```

---

### 2. Run the Automation Script

```
python image_preview_test.py --url "https://www.pixelssuite.com/convert-to-png" --slow-mo-ms 2000
```

---

## 📊 Output

### ✔ CSV File

* `execution_results.csv` contains:

  * File type
  * File path
  * Preview detection result
  * Test status (PASS/FAIL)
  * Screenshot path

---

### ✔ Screenshot

* Saved in:

```
results/preview_pass.png
```

---

## ✅ Test Result

* Preview detected: **True**
* Status: **PASS**

---

## 🧠 Assumptions

* The system should display a preview after uploading a valid PNG image
* The preview section contains visible image elements

---

## ⚠️ Limitations

* Only frontend functionality is tested
* Backend, performance, and security testing are not included

---

## 👨‍💻 Author

* Registration Number: IT23394506

---

## 📌 Notes

* Ensure internet connection is active before running the script
* The script automatically creates a PNG file if not available
* Use `--slow-mo-ms` to visually observe test execution

---
