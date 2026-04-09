# 📊 Enterprise Excel Data Cleaner & Analyzer

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-2.0-green)](https://pandas.pydata.org)
[![License](https://img.shields.io/badge/License-MIT-yellow)](LICENSE)

## 🎯 What is this?

An **Enterprise-grade Excel Data Cleaner and Analyzer** that automatically detects phone numbers, purchase amounts, cleans data, calculates risk scores, segments customers, and generates AI-powered business insights with visual charts and color-coded reports.

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🔍 **Smart Column Detection** | Automatically finds phone and purchase columns |
| 🧹 **Data Cleaning** | Removes duplicates, fixes phone numbers, handles missing values |
| 📊 **Customer Segmentation** | Premium, VIP, Regular, Low categories based on purchase amount |
| ⚠️ **Risk Scoring System** | Calculates risk based on invalid phone, duplicates, low purchase |
| 📈 **AI Business Insights** | Generates business health score (0-100) with grade |
| 🎨 **Color-Coded Output** | Highlights rows by customer type and risk level |
| 📉 **Auto Chart Generation** | Creates revenue by customer type bar chart |
| 🔒 **License Protection** | Built-in license key verification system |

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python 3.10 | Core programming |
| Pandas | Data manipulation |
| Tkinter | GUI interface |
| OpenPyXL | Excel styling & charts |
| Matplotlib | Chart generation |
| NumPy | Numerical operations |
| Hashlib | License key security |

## 📋 What It Does

### Input (Your Excel File)
| Name | Phone | Purchase Amount |
|------|-------|-----------------|
| John | 01712345678 | 500 |
| Jane | 12345 | 2000 |
| Bob | invalid | 100 |

### Output (Cleaned File with 4 Sheets)

**Sheet 1: Cleaned Data** (Color-coded)
| Name | Phone | Purchase Amount | Customer Type | Risk Level |
|------|-------|-----------------|---------------|------------|
| John | 01712345678 | 500 | VIP | Low |
| Jane | 12345 | 2000 | Premium | High |
| Bob | (empty) | 100 | Low | High |

**Sheet 2: Duplicates** - Lists all duplicate phone records
**Sheet 3: Invalid Rows** - Lists rows with invalid phone numbers
**Sheet 4: AI Insights** - Business health score, grade, and metrics + Bar chart

## 🚀 How to Use

### Installation

```bash
# Clone repository
git clone https://github.com/jasoncl007/excel-data-cleaner-analyzer.git

# Install dependencies
pip install pandas numpy openpyxl matplotlib

# Run application
python excel_cleaner.py
