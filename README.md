# qr-code-generator
qr code generator

This Python code generates a QR code image for a given URL (web address) provided by the
user. Here's a step-by-step explanation of how it works:
1. import qrcode: This line imports the "qrcode" library, which allows you to create QR
codes.
2. def generate_qrcode(text):: This line defines a function called
generate_qrcode that takes one parameter called text. This parameter represents
the text (in this case, a URL) for which you want to generate a QR code.
3. Inside the generate_qrcode function:
○ qr = qrcode.QRCode(...): This code initializes a QR code object (qr) with
specific settings:

■ version = 1: Specifies the version of the QR code (in this case,
version 1).

■ error_correction = qrcode.constants.ERROR_CORRECT_L:
Sets the error correction level to low (L).

■ box_size = 10: Determines the size of each small square box in the
QR code.

■ border = 4: Sets the border size around the QR code.
○ qr.add_data(text): Adds the input text (the URL) to the QR code.
○ qr.make(fit=True): Generates the QR code based on the provided settings
and input text. The fit=True parameter ensures that the QR code adjusts its
size to fit the content.

○ img = qr.make_image(fill_color="black", back_color="white"):
Creates an image (img) representation of the QR code. It sets the fill color to
black and the background color to white.

○ img.save("qrimg001.png"): Saves the generated QR code image as
"qrimg001.png" in the current directory.

5. url = input("Enter your URL: "): This line prompts the user to enter a URL
and stores it in the variable URL.

6 generate_qrcode(url): Calls the generate_qrcode function, passing the
user-entered URL as an argument. This generates the QR code for the provided URL

This Project is Created By Jyotirmay Chowdhury.
https://jyotirmaychowdhury.pages.dev/
and saves it as "qrimg001.png" in the same directory as the script.

In summary, this code allows the user to input a URL, and it then creates a QR code for that
URL with specific settings saves it as an image, and names it "qrimg001.png" in the current
directory. 

This QR code can be used for various purposes, such as linking to websites or
sharing information digitally.
