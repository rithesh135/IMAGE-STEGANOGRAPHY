# IMAGE-STEGANOGRAPHY
ENCODING AND DECODING HIDDEN DATA WITHIN AN IMAGE FILE

**Project Prerequisites:**
To build this Python Image Steganography project, we will need the following libraries:
1. **Tkinter** – To create the GUI
2. **PIL** – Python Image Manipulation library. It is used to perform operations on images in python.
While the Tkinter library comes pre-installed with Python, the PIL library does not, so you will have to run the following command to install it.
**python -m pip install pillow**

**Project File Structure:**
Here are the steps you will need to execute to build this Image Steganography project in Python:
1. Initializing the root window and placing all components in it
2. Defining all the backend encryption and decryption functions
3. Defining the GUI functions of decoding and encoding

**Initializing the root window and placing all components in it:**

# Initializing the window of Python Image Steganography Project
root = Tk()
root.title('ProjectGurukul Image Steganography')
root.geometry('300x200')
root.resizable(0, 0)
root.config(bg='NavajoWhite')
Label(root, text='ProjectGurukul Image Steganography', font=('Comic Sans MS', 15), bg='NavajoWhite',
wraplength=300).place(x=40, y=0)
Button(root, text='Encode', width=25, font=('Times New Roman', 13), bg='SteelBlue', command=encode_image).place(
x=30, y=80)
Button(root, text='Decode', width=25, font=('Times New Roman', 13), bg='SteelBlue', command=decode_image).place(
x=30, y=130)
# Finalizing the window
root.update()
root.mainloop()

