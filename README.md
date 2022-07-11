# ASSEMBLY PROJECT
Semester 2 - 21_22 - Mr.Thai Hung Van.\
Class: 20_5 - HCMUS.
# MEMBERS
1. Nguyen Huu Phuc - 20120161
2. Hoang Thu Thuy  - 20120382
## I. Project description
This is a x86 assembly language program to check the status of the keyboard lights and performs the following functions:
1. If both CapsLock and NumLock lights are on: Display the machine's time on the screen.
2. If only CapsLock light is on: Enter a string of up to 80 characters, change all lowercase characters in that string to uppercase and display the resulting string to the screen.
3. If only NumLock light is on: Enter 2 natural numbers with value up to 32 767;  calculate sum, difference, product, quotient and display the result.
4. If both CapsLock and NumLock lights are off: Display the corresponding greeting message (Good morning/afternoon/evening).
## II.How to run the program
1. First you need to download [DOSBox](https://www.dosbox.com/download.php?main=1) and [TASM](https://www.pconlife.com/viewfileinfo/tasm-1-4-windows-7-windows-8-64-bit-techapple-net-exe/) (or if you are still having trouble, check this [tutorial video](https://www.youtube.com/watch?v=JH-OCVkj3EY)). 
2. After install TASM, open folder *TASM* and move source code file *Final.asm* into it.
3. Open short cut *Tasm AutoMount Manual Edit-Tlink-TD* in folder *TASM 1.4*
4. Type the following DOSBox commands:
    - tasm final
    - tlink final
    - final.exe
5. Notice: if your laptop keyboard does not have ScrollLock, you can use *On-Screen Keyboard* app that is always available in windows operating system.
## III. Special knowledge
> **Get system time:** 
    - Int 21h, 2Ch.
    - Input: AH = 2Ch
    - Output: CH = hour, CL = minute, DH = second
> **Get shift status:** 
    - Int 16h, 2h
    - Input: AH = 2h
    - Output: AL = Shift status. [Details](http://vitaly_filatov.tripod.com/ng/asm/asm_027.3.html).



## IV. Demo Video
- <https://www.youtube.com/watch?v=mIuBjXyFAFE>
