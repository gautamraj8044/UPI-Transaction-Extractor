# UPI Transaction Extractor: OCR-Based Data Parsing Tool  

## 📄 **Overview**  
The **UPI Transaction Extractor** is a Python-based project that automates the process of extracting transaction details from UPI payment screenshots. It leverages image preprocessing, Optical Character Recognition (OCR) using PaddleOCR, and text parsing techniques to identify and structure details like transaction status, amount, date, time, UPI ID, sender, and recipient. The results are saved in a structured JSON format for easy use.  

---

## 🛠 **Features**  
- Preprocesses images to enhance OCR accuracy.  
- Extracts text from images using PaddleOCR.  
- Parses and identifies key transaction details:
  - Transaction status (e.g., Paid Successfully, Failed).  
  - Amount, Date, and Time.  
  - UPI ID and type (e.g., Google Pay, Paytm, PhonePe).  
  - Sender and recipient information.  
- Saves structured transaction data as a JSON file.  

---

## 🚀 **How It Works**  
1. **Image Preprocessing**:  
   - Resizes the image.  
   - Removes noise and converts the image to grayscale.  
   - Applies adaptive thresholding for better text extraction.  

2. **Text Extraction**:  
   - Uses PaddleOCR to extract textual data from the preprocessed image.  

3. **Text Parsing**:  
   - Extracts specific details like amount, UPI ID, date, and more using regular expressions.  

4. **Data Structuring**:  
   - Organizes the parsed data into a standard JSON format.  

5. **JSON Export**:  
   - Saves the structured transaction details as a JSON file for easy storage or further analysis.  

---

## 🛠 **Requirements**  
- Python 3.8+  
- Libraries:
  - `opencv-python`  
  - `paddleocr`  


---

## 🔧 **Installation**  

1. **Clone the Repository**  
   ```bash  
   git clone https://github.com/your-username/upi-transaction-extractor.git  
   cd upi-transaction-extractor  
   ```  

2. **Install Dependencies**  
   ```bash  
   pip install opencv-python paddleocr  
   ```  

---

## 📋 **Usage**  

1. Place the UPI transaction screenshot in the project directory.  
2. Update the `images` variable in the script with the image filename.  
3. Run the script:  
   ```bash  
   python OCR_assigment.py  
   ```  

4. The extracted transaction details will be displayed on the console and saved as `transaction_details.json`.  

---

## 🧪 **Example Output**  

```json  
{  
    "transaction_status": "Paid Successfully",  
    "amount": "₹1500",  
    "date": "12 April 2024",  
    "time": "10:30 AM",  
    "UPI type": "Google Pay",  
    "UPI ID": "example@upi",  
    "To": "John Doe",  
    "From": "Jane Smith"  
}  
```  

---




## 🤝 **Contributing**  
Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-username/upi-transaction-extractor/issues).  

---

## 📧 **Contact**  
For any inquiries or support, please reach out to:  
- **Email**: gautamraj8044@gmail.com
- **GitHub**: [gautam8044](https://github.com/gautam8044)  

---  

✨ **Happy Extracting!** ✨  
