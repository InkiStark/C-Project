# < IP converter >

## Description 

_‘Ip converter’_ is an application made in C language that allows the user to convert an IP address in decimal form to binary and vice versa.<br>
The program accepts only an IP in a specified format which is xxx.xxx.xxx.xxx containing numbers from 0 to 255 while in decimal and xxxxxxxx.xxxxxxxx.xxxxxxxx.xxxxxxxx allowing 0 and 1 only while in binary format.<br>
It is an academic project made for educational purposes , aiming to be a very useful and easy tool both for students and network professionals.<br> 
Also as the code is freely distributable we hope that it will be a good learning experience for beginners or anyone wishing to have a taste of programming on a basic level.<br>

## Instalation

In order to use our code, someone would need a compiler programm for C language. Few examples are [Dev-C++](https://sourceforge.net/projects/orwelldevcpp/),[Visual Studio Code](https://code.visualstudio.com/download), or can use and online compiler (e.x https://www.programiz.com/c-programming/online-compiler/). 
After having a compiler, next step would be to copy the code and paste it into your compiler.

## Usage

The use of the code is quite easy to follow. There are three options for this project for the user to decide.

![](images/Execute.png) 

+ As you can see, _Option 1_ requires from the user,
firstly to press #1 in order to start that option. After pressing #1 and enter, it will be required to insert a 32 bit binary IP address in order to covert it into decimal form,as displayed in the image bellow.

![option1](https://user-images.githubusercontent.com/116667541/215594162-f8741161-184c-415e-94a0-88c74cdfb522.png)

+ The user can insert a binary number as an IP address (we choose a random binary number for the display). The result will be an IP address in decimal form, and the programm will get back to the menu in order to choose another option.

![result1](https://user-images.githubusercontent.com/116667541/215596599-1fa57167-22a1-48c5-8f73-3901d77a9c74.png)

+ Moving on, we can choose _Option 2_ so we can convert the IP address the other way around,meaning from decimal form to binary.As the user chooses _Option 2_ it will be asked from him to enter an IP address in decimal form.The user can insert an IP address in order to convert it into a binary form and back to the menu in order to choose _Option 3_ to terminate the programm.

![option3](https://user-images.githubusercontent.com/116667541/215598328-7b736d76-43b7-4d35-ad31-048a5a93d1e9.png)





## Credits

Authors names : InkiStark,ThTsiavos,PortalWinter 
- Date : 03/02/2023
- Title of program/source code : IP converter
- Code version :
- Type : Source code
- Web address or publisher (We don't have one)

## License 

Free to use.

## Badges

## Tests


+ In order to verify the functionality of the application, we used the following scenarios, resulting in a successful pass for all
Case 1 – IP conversion - The user inputs an IP address following the specified format,
expected behavior is to return an IP from the opposite form and show the expected text:

<ul>
<li>IP1: 192.168.3.1</li> <li>IP2: 10.24.20.20</li> <li>IP3: 0.0.0.0</li>
<li>IP4: 10111100 11101100 00001111 00000001</li>
<li>IP5:00001111 10101010 01010101 11111111</li>
<li>a)    Decimal to Binary -   Result = All Pass</li>
<li>b)    Binary to Decimal –    Result = All Pass</li>
</ul>      

+ Case 2 – Menu – The user chooses a menu from the specified options and an invalid option which is a number , a symbol and an alphabet as well as combinations of all.
Expected behavior is to show text:
A) “Enter 32-bit IP address in dotted decimal notation(...):” if input is 1 – Result = Pass
B) “Enter 32-bit Ip address in binary form (xxxxxxxx.xxxxxxxx.xxxxxxxx.xxxxxxxx): "if input is 2 – Result = Pass
C) "I don't know the option “if input is anything else Result = Fail – the choice number was shown incorrectly (Changed the code to show “I don’t know this option “instead
D) ”Quit the program: if option 3 and close the application– Result = Pass

+ Case 3 – Invalid user inputs after the initial menu choice – Expected Behavior is to show the correct error messages
A)    Option 2 – Decimal to Binary – 
i)The user inputs an invalid number, alphabet or symbol – Result = Fail (No error message, no escape sequence, program crashed)
ii)The user inputs a number in invalid size (too short, too long) – Result = Pass
      B)Option 2 – Binary to Decimal –
I)The user inputs a number that is not 1 or 2 ,and also an alphabet or symbol – Result = Pass
ii)The user input a binary number of invalid size – Result = Fail (A 9 digit number was accepted and result was returned)
