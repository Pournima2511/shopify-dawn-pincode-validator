# Shopify Pincode Validator – Dawn Theme

## 🧩 Overview

This project adds a **Pincode Validator** section to the product page using Shopify's **Dawn theme**. The validator checks user-entered pincodes against a list stored in **Google Sheets**.

---

## ✨ Features

- A custom `pincode-validator` section for product pages.
- Real-time validation using Google Sheets (converted to JSON API).
- Displays "Delivery Available" or "Delivery Not Available" based on validation.
- Clean and responsive layout using minimal CSS/JS.

---

## 💡 Coding Approach

### 🔹 Section Creation

- A new section `pincode-validator.liquid` was created under `/sections/`.
- Contains HTML input field and button to check availability.
- JavaScript fetches the JSON data and validates the pincode.

### 🔹 Google Sheets Integration

- Used [opensheet.elk.sh](https://opensheet.elk.sh) to convert Google Sheet to public JSON.
- Google Sheet format:
Pincode
400001
400002

- Example URL:
https://opensheet.elk.sh/YOUR_SHEET_ID/Pincodes


### 🔹 Shopify Theme Integration

- Since Shopify’s **Dawn theme** uses `product.json`, the section was added directly to the product page.
- Due to a limitation (`Cannot render sections inside sections`), the custom section was added after `main-product`.


## 📂 Folder Structure
/sections └── pincode-validator.liquid /templates └── product.json


## 👩‍💻 Developer

**Pournima Madan Gade**  
Web Developer

