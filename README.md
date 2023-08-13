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
:white_check_mark:Initializing the root window and placing all components in it

:white_check_mark:Defining all the backend encryption and decryption functions

:white_check_mark:Defining the GUI functions of decoding and encoding

**Initializing the root window and placing all components in it:**

	.callout_inforoot = Tk()

	.callout_inforoot.title('Proton Image Steganography')

	.callout_inforoot.geometry('300x200')

	.callout_inforoot.resizable(0, 0)

	.callout_inforoot.config(bg='NavajoWhite')

	.callout_infoLabel(root, text='Proton Image Steganography', font=('Comic Sans MS', 15), bg='NavajoWhite',

	.callout_infowraplength=300).place(x=40, y=0)

	.callout_infoButton(root, text='Encode', width=25, font=('Times New Roman', 13), bg='SteelBlue', command=encode_image).place(x=30, y=80)

	.callout_infoButton(root, text='Decode', width=25, font=('Times New Roman', 13), bg='SteelBlue', command=decode_image).place(x=30, y=130)

	.callout_inforoot.update()

	.callout_inforoot.mainloop()

**Explanation:**

We will assign the Tk() class to the root variable to initialize the window. The methods and attributes that need to be set during initializing are:

The .title() method is used to give a title to the window.

The .geometry() method is used to define the initial dimensions of the window in pixels.

The .resizable() method specifies whether the user will be allowed to resize the window or not. It takes only truth and falsy values in the form of (width, height).

The .config() method is used to configure other attributes of the window, such as the bg attribute which denotes the colour of the background of the window.

The .update() and .mainloop() methods put the window in a loop to prevent it from closing until told otherwise.

**Note:**

These two lines will be the last lines in a GUI script that the Python interpreter will run in it.
The Label class is used to create a Label on the window that displays static text on the window. Its parameters that need to be set during assignment are:

.callout_warn The master parameter, the positional argument root here, is the parent widget this widget is associated with.
	The text parameter refers to the text that will be displayed on the label.
	The font parameter defines the font family, size and effects that will be applied to the text displayed on the label.
	The wraplength parameter specifies the number of pixels after which the text has to be moved to the next line.
The Button class is used to add a button to the window that runs a function when it is pressed. Its parameters are:
	The command parameter is used to define the function that will run when the button is pressed. You will not need the lambda keyword if the function to run does not need any arguments.
The .place() method is used to place a widget on its parent widget as though the parent is a Cartesian Plane, with the Northwest corner being the origin of that plane.
	The x,y parameters define the horizontal and vertical offsets of the widget, respectively.
	The relx,rely parameters define the horizontal and vertical offsets as a decimal number between 0.0 and 1.0



