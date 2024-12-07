# UPI Payment QR Code Generator

This Python script helps you generate UPI payment QR codes that can be used with UPI-enabled apps like Google Pay, PhonePe, or Paytm. It allows you to customize the payment details such as recipient name, UPI ID, amount, currency, and transaction note.

---

## Features

- Generate a QR code for UPI payments effortlessly.
- Customizable fields include:
  - UPI ID
  - Recipient name
  - Payment amount
  - Currency (default: INR)
  - Transaction note
- Works with UPI-enabled apps like Google Pay, PhonePe, and Paytm.
- Options to display the QR code or save it as an image file.

---

## Prerequisites

1. **Python** (Ensure Python 3.x is installed).
2. Install the required library using the following command:
   ```bash
   pip install qrcode
   pip install pillow
   pip install ipython

   
##How to Use

3Step 1: Clone or Download the Script
Download the script file to your local machine.

#Step 2: Run the Script
Run the script in your Python environment (e.g., IDLE, Jupyter Notebook, or VS Code). You'll be prompted to provide the following details:

 Enter the UPI ID: (e.g., recipient@upi)
 Enter the amount to pay: (e.g., 100)
#Step 3: QR Code Generation
 The script generates a QR code based on the input provided. You can:

 Display the QR code directly in the output (suitable for Jupyter Notebook or IDLE).
 Save the QR code as an image file by uncommenting the relevant lines in the code. 

 #Example input
 Enter your UPI ID: recipient@upi
 Enter the amount to pay: 150

##Saving QR Code as an Image
 #To save the QR code:

##Uncomment the line in the script:
 #python
#Copy code
google_pay_qr.save('googlepay_qr.png')
#After running the script, the QR code will be saved as googlepay_qr.png in the same directory as the script.


##Using the Script in Google Colab
 If you're running the script in Google Colab:

  Ensure you use display(google_pay_qr) to display the QR code.
  Download the saved QR code file to your local system if needed.


##Advantages
 #Convenience: Automates the process of generating UPI QR codes, saving time.
 #Customizable: Allows you to specify recipient details and transaction parameters.
 #Compatibility: Works seamlessly with popular UPI apps like Google Pay, PhonePe, and Paytm.
 #Portability: QR codes can be saved and shared easily.
 #Educational: Learn how to work with Python libraries for generating QR codes.


##Additional Customization
 #To generate QR codes for other UPI apps:

 #Modify the URL structure to match the app's requirements. For example:
  python
  Copy code
  #phonepe_url = f'upi://pay?pa={upi_id}&pn={recipient_name}&am={amount}&cu={currency}&tn={transaction_note}'
  
 #Create QR codes using:
 
  python
  Copy code
  #phonepe_qr = qrcode.make(phonepe_url)
  #Save or display as needed.
