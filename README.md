# To-do-list
Listbox: We will be using Python Tkinter Listbox to show multiple tasks stacked one after another. And tasks can be selected when clicked on it.
Scrollbars: Scrollbars will help us to stack plenty of data without worrying about the space on the window. The Tasks can be accessed by scrolling the Listbox.
Frame: Frame will be used to put widgets like Listbox and Scrollbars inside it. This will give us control to align Listbox to the left & scrollbar to the right so that they both appear parallel & perfect.
Buttons: We will add two button widgets on the window. One is to add more tasks in Listbox and the other is to delete tasks from Listbox.
Entry box: Users will type the task in the entry box which further will be displayed in the Listbox.
Messagebox: The Python Tkinter message box is used to display an error message when the user clicks on the add button with an empty entry box.

# Code-Explainantion

Step 1 : Import Modules

Before we start using Tkinter, we need to call Tkinter for use. so we import the module. Here * means everything. So we are importing everything from Tkinter then in the second line we have imported message box from Tkinter.

Step 2: Create & Configure Window
After importing module, we will create a window so that we can place widgets on it.

ws is used to initialize Tk(). From now ws will be called as the parent window. All other widgets will be placed on it.
ws.geometry(‘width x height + x-position+ y-position’)
All the values provided must be integers.
the width refers to the horizontal space of the window.
height refers to the vertical space of the window.
x-position refers to the position of the window on the display over the x-axis.
y-position refers to the position of the window on the display over the y-axis.
the title will add a title to the window. In our case, we have provided our website name as a title. You can find the title on the top left of the window next to feather.
config is used to provide background color to the window.
resizable accepts boolean values. Since the boolean values are provided false for both height and width that means the window can’t be resized. To know more about resizable please read our blog on python Tkinter windows size.
ws.mainloop() holds the screen so that we can see the window. It is an infinite loop. screen pops up and then disappears but with this infinite loop this process of appearing & disappearing keeps on happening very fast. And we keep on seeing the updated window.

Step 3: Creating a frame
n this section we will understand why we have used frames as a first widget in our code.

1.Frame widgets are used to hold other widgets.\n
2.They help in keeping & maintaining user interface (UI) & user experience (UX) clean & organized.\n
3.Moving forward we will place Listbox, scrollbars & buttons inside the frame.\n
4.So in this way frame will act as an additional window over the parent window.
5.Another benefit of placing a frame is now we will add scrollbars to the frame and that solves our purpose.
6.Scrollbars are no easy to place but using frames we can do it in no time.
7.pady=10 means we have added extra padding around the frame from outside

Step 4: Adding Listbox
n this section, we will learn why and how we have used Listbox on the window.

1.lb is the variable name for storing Listbox.
2.Listbox is placed on the frame window.
3.width: Horizontal space provided is 25.
4.height: 8 rows in the vertical position are provided.
5.font: Times New Roman font is provided with 14 sizes.
6.bd = 0 refers to the border is zero
7.fg is the foreground color or the text color.
8.highlightthickness=0 every time the focus is moved to any item then it should not show any movement that is value 0 value is provided. by default it has some value.
9.selectbackground it decides the color of the focused item in the Listbox.
10.activestyle=”none” removes the underline that appears when the item is selected or focused.
11.geometry manager used is pack()
12.side=LEFTthis will keep the Listbox to the left side of the frame. We did this on purpose so that we can assign the right position to scrollbars.
13.fill=BOTH this will fill the blank space in both the directions that are x and y

Step 5: Adding dummy data

