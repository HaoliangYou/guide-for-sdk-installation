# guide-for-sdk-installation: Haoliang You
University of Pennsylvania, ESE 5190: Intro to Embedded Systems, Lab 2A

    Haoliang You
       haolyou@seas.upenn.edu
    Tested on: ROG Zephyrus (16-inch, 2022), Windows 11

 Building on MS Windows
1. Installing the Toolchain
First, we are supposed to install these 5 extra tools:
(1)Arm GNU Toolchain
(2)CMake
(3)Building Tools for Visual Studio 2022
(4)Python 3.10
(5)Git
 
1.1 Installing Arm GNU Toolchain
Be sure to tick all the ticks  
![a](图1)

1.2 Installing CMake
You are supposed to choose "Add CMake to the system PATH for all users" when installing CMake
![a](图2)

1.3 Installing Build Tools for Visual Studio 2022
Be sure to install the C++ build tools only
![a](图3)

1.4 Installing Python 3.10
You should tick the "Add Python 3.10 to PATH" box. Be sure that python is installed for all users. 
What is more, be aware to disable the MAX_PATH length limit at the end of installing.
![a](图4)

1.5  Installing Git
Ensure that you have changed the default editor away from vim to  to Notepad.
Be sure you tick the checkbox to allow Git to be used from 3rd-party software. 
You are supposed to check the box "Checkout as is, commit as-is". Then be sure to select "Use Windows'default console window", and tick the "Enable experimental support for pseudo consoles" checkbox when installing the Git.
![a](图5)

2. Getthing the SDK and examples
Create the log in C:\Users\10233\Downloads for myself.
Input the following code in the Terminal of the PC.
![a](图6)
You will get the result as the following pic if it works well.
![a](图7)

3. Building "Hello World" from the Command Line
Open a Developer Command Prompt window from the Windows Menu.
Select Windows->Visual Studio 2022 -> Developer Command Prompt for VS 2022 
After that, set the path as the following pictures:
![a](图8)

Then, close your current Command Prompt window and open again. Set the environment variables as the following pic.
![a](图9)

You will get the result like the following pic if you build successfully.
![a](图10)

4.Building "Hello World" from Visual Studio Code
First, install Visual Studio Code and build your projects inside the that environment rather than from the command line
Select Windows -> Visual Studio 2022 -> Developer Command Prompt for VS2022 from the menu and type C:> code to open the Visual Studio Code with all the correct environment variables
Then install the CMake Tools extension. Click the "Add Item" and set  PICO_SDK_PATH as ....\pico-sdk.
You are also supposed to find "Cmake: Generator" and type in "NMake Makefiles".
Finally, you can have a try to build it.

5. Flashing and Running "Hello World"
Press BOOTSEL andpull it in your usb port and reset you RP2040.
You can check the detailed information of your serial line in Windows Device Manager as follows.
![a](图11)
Open the PUTTY and set the variable like this.
![a](图12)
Click save and open, you will see the serial as follows!
![a](图13)


