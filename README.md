# Safety-Scan
🛡️ Safety Scan

Safety Scan is an AI-powered application that analyzes product label images to determine whether a product is safe to use or expired.
It uses OCR (Optical Character Recognition) and intelligent date inference to extract manufacturing and expiry dates—even when labels are unclear or partially unreadable.

🚀 Features

-- 📸 Image-based scanning of product labels

-- 🔍 Robust OCR using EasyOCR & Tesseract

-- 📅 Smart date extraction (handles noisy OCR, missing years, and multiple formats)

-- 🧠 Date inference logic for real-world labels

-- ✅ Automatic safety check (Safe / Expired / Unknown)

-- 🌐 Interactive web interface using Gradio

-- 🧩 Modular backend for easy API integration

🧠 How It Works

-- 📸 Upload a product image

-- The image is processed using OCR

-- Manufacturing & expiry dates are:

-- Extracted using regex

-- Cleaned and normalized

-- Inferred when partially missing

The system compares the expiry date with today

A safety status is returned

🏗️ Tech Stack
--> Backend

-- Python

-- EasyOCR

-- DateParser

-- NumPy

-- Pillow

--> Frontend

-- Gradio (Web UI)

-- Pytesseract

--> Deployment & Tools

-- Google Colab

-- Ngrok (for exposing backend & frontend)

-- GitHub

📂 Project Structure

Safety-Scan/
│
├── backend.ipynb        # OCR, date extraction, safety logic
├── frontend.ipynb       # Gradio-based user interface
├── README.md            # Project documentation


⚠️ Safety Logic

✔ Safe to use → Today ≤ Expiry Date

❌ Not safe to use → Today > Expiry Date

❓ Unknown → Expiry date not detected

🧪 Example Output

Input :

<img width="225" height="212" alt="Screenshot 2025-09-27 142817" src="https://github.com/user-attachments/assets/5fe6d3eb-3517-4c09-a8b6-f0f280a827fb" />

Output :

{
  "Manufacturing Date": "2024-06-17",
  "Expiry Date": "2026-06-17",
  "Safety Status": "Safe to use"
}



