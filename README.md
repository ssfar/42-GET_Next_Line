# 42-GET_Next_Line
A function able to read content line by line without knowing previously the length of them.

Subject : [English](https://github.com/ssfar/42-Subjects.pdf/blob/master/get_next_line.en.pdf) - [Français](https://github.com/ssfar/42-Subjects.pdf/blob/master/get_next_line.fr.pdf)

Grade 100/100  
Bonus 25/25 :  
 :heavy_check_mark: Only one static variable | :heavy_check_mark: Multiple file descriptors handeling

#### Objectives :
• Filedescriptors   
• Buffering  
• Basic parsing
#### Skills :
• Imperative programming  
• Rigor  
• Algorithms & AI   
 
#### Here is the function prototype
![gnl](https://user-images.githubusercontent.com/45463065/86376673-a39fff00-bc87-11ea-8ab7-e61522c957fc.png)

## How to use

This functions can be used in a loop to read an entire file.  
It is also able to manage multiple file descriptor without losing the reading thread on each of the descriptors.

### Input

The first parameter is the file descriptor that will be used to read.  
The second parameter is the address of a pointer to a character that will be used to save the line read from the file descriptor.

### Output

In case of a succesfull read, the given pointer to a character is allocated whit malloc() and the line read is stored inside the allocated area whitout the trailing newline.  
The return value can be 1, 0 or -1 depending on whether a line has been read, when the reading has been completed, or if an error has happened respectively.
