Image Encryption Tool
This is a simple Python tool that allows you to encrypt and decrypt images using pixel manipulation. The encryption process modifies the pixel values of an image based on a user-defined integer key, while the decryption process restores the original image using the same key.

Features
Encrypt images by shifting pixel values.
Decrypt images to retrieve the original content.
User-friendly interface for inputting file paths and keys.

Requirements
Python 3.x
Pillow library (for image processing)

Installation
You can install the required library using pip:

pip install pillow

Usage
Prepare an Image: Ensure you have an image file (e.g., image.jpg) that you want to encrypt or decrypt.

Run the Program: Execute the script using Python. The program will prompt you for input.

Example Interaction
Step 1: Encrypt the Image

Would you like to (E)ncrypt or (D)ecrypt an image? E
Enter the path to the image file: C:\Users\YourName\Desktop\image.jpg
Enter the path to save the new image: C:\Users\YourName\Desktop\encrypted_image.jpg
Enter an integer key for encryption/decryption: 50
Step 2: Decrypt the Image

Would you like to (E)ncrypt or (D)ecrypt an image? D
Enter the path to the image file: C:\Users\YourName\Desktop\encrypted_image.jpg
Enter the path to save the new image: C:\Users\YourName\Desktop\decrypted_image.jpg
Enter an integer key for encryption/decryption: 50

Code Overview

Functions
encrypt_image(image_path, output_path, key):

Encrypts an image by adding the key to each pixel's RGB values.
decrypt_image(image_path, output_path, key):

Decrypts the encrypted image by subtracting the key from each pixel's RGB values.
image_cipher():

Main function that interacts with the user to perform either encryption or decryption based on user input.
Notes
Ensure that the key used for decryption is the same as the one used for encryption.
The program operates in a basic manner and is intended for educational purposes.
The pixel manipulation method used here is not intended for secure encryption; it serves as a simple example of how to manipulate image data.

License
This project is open-source and available under the MIT License.
