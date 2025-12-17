# Safety-Scan
🛡️ Safety Scan

Safety Scan is an AI-powered application that analyzes product label images to determine whether a product is safe to use or expired.
It uses OCR (Optical Character Recognition) and intelligent date inference to extract manufacturing and expiry dates—even when labels are unclear or partially unreadable.

🚀 Features

📸 Image-based scanning of product labels

🔍 Robust OCR using EasyOCR & Tesseract

📅 Smart date extraction (handles noisy OCR, missing years, and multiple formats)

🧠 Date inference logic for real-world labels

✅ Automatic safety check (Safe / Expired / Unknown)

🌐 Interactive web interface using Gradio

🧩 Modular backend for easy API integration

🧠 How It Works

Upload a product image

The image is processed using OCR

Manufacturing & expiry dates are:

Extracted using regex

Cleaned and normalized

Inferred when partially missing

The system compares the expiry date with today

A safety status is returned

🏗️ Tech Stack
Backend

Python

EasyOCR

DateParser

NumPy

Pillow

Frontend

Gradio (Web UI)

Pytesseract

Deployment & Tools

Google Colab

Ngrok (for exposing backend & frontend)

GitHub
