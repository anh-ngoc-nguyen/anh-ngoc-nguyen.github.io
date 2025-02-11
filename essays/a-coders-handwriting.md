---
layout: essay
type: essay
title: "A Coder’s Handwriting"
# All dates must be YYYY-MM-DD format!
date: 2025-02-10
published: true
labels:
  - Software Engineering
  - C/C++
  - Typescript
  - Coding Standards
---

<div style="text-align: center;">
  <img src="../img/coding-standards.jpeg" alt="Coding Styles" style="width: 300px; border-radius: 15px; display: block; margin: 0 auto;">
  <p style="margin-top: 10px;">Source: Medium</p>
</div>

<hr>

## Coding Style is a Matter of Choice
Like with any written language that is transcribed to paper, the stylistic characteristics and choices are ultimately up to the writer. How they choose to format their writing may depend on their audience such as if they are documenting for themself only or for others to read as well. One may choose to incorporate cleaner letters for legibility having prior knowledge that others may view their work. On the other hand, they may choose efficiency over neatness if the writing is only for their eyes to cut costs on time. Although the prompt can be the same, there is a time and place where one is more beneficial than the other. This is generally how I feel about personal coding standards and preferences.

## Encountering Coding Standards for the First Time
In my experience, I had not encountered any coding standard requirements for my programs up until last semester when I took Program Structure, a C/C++ centered course. Throughout the class, all of the assignments needed to be formatted in a specific way, or else points would be docked off for stylization. I found these conditions tedious and time-consuming considering these efforts were done in a Linux terminal emulator. In other words, simple keyboard inputs such as “Ctrl + C”, “Ctrl + V”, or even “Tab” rendered it useless and did not provide any helpful shortcuts as it normally would. An example of the style I had to adhere to can be seen below.
```
/*****************************************************************
//  FUNCTION NAME: is_multiple3 
//  DESCRIPTION: This function will determine all the numbers 
//               that need to be printed is a multiple of 3 or
//               not.
//  PARAMETERS:  number (int) uses the value of all the
//               integers that needed to be printed determined.  
//  RETURN VALUES:  1 : The number is a multiple of 3
//                  	      0 : The number is not a multiple of 3
***************************************************************/
int is_multiple3(int number)
{
    if (number ==0)
    {
         return 0;
    }    
    if(number % 3 == 0)
    {
        return 1;
    }
    return 0;
}
```
As you can observe, every function that was made needed a block of comments that described the various aspects of it. In terms of braces, it was necessary to place them on a new line and each indentation was made specifically with 4 spaces, not “Tab”. In combination with the complex setbacks of keyboard input, the laborious hassle significantly outweighed the potential readability benefits.

## A Smoother Experience with ESLint
In terms of utilizing ESLint to “autocorrect” my programming through VSCode, the process was not as grueling as it initially seemed. Although the ESLint coding standards were more strict and required more attention to detail, my experience with adhering to them was far less taxing than using the Linux terminal. This was most likely due to the console notifying me specifically of the syntax errors I needed to fix as opposed to having to manually keep track of the standards myself. While it did not necessarily aid me in learning how to code better, it did make certain blocks more legible and aesthetically pleasing to the eye as shown below.
```
function sumFor(list: number[]): number {
  let sum: number = 0;
  for (let i = 0; i < list.length; i++) {
    sum += list[i];
  }
  return sum;
}
console.log(sumFor([1, 2, 3, 4]));

function sumWhile(list: number[]): number {
  let i: number = 0;
  let sum: number = 0;
  while (i < list.length) {
    sum += list[i];
    i++;
  }
  return sum;
}
console.log(sumWhile([1, 2, 3, 4]));
```
Instead of functions being separated by chunks of comments like in my previous example, they are structured in a certain manner that still divides it in an orderly fashion. While some may say that ESLint errors can be painful to fix due to miniscule mistakes such as having spaces in particular areas of the code, it can provide useful habits, especially in larger projects. 

## Balancing Standardization and Personal Preference
I do not necessarily have a vendetta against the standardization of code, however, I do believe that there is a time and place for them. As mentioned earlier, I believe that a coder’s typing style is very similar to one’s handwriting on paper. Everyone has unique methodologies to their writing but sometimes one form may be more useful than the other based on the circumstances. If someone is working on a website for themself where no one else will need to see behind the scenes, then by all means they should code freely however they choose to. In a broader scenario, however, large-scale projects where multiple people are coordinating together require basic formatting rules so that everyone is on the same page. It is only a matter of situational awareness and purpose, as such with handwriting. 
