## Cnotes
# Day 1
Scratch: say (Hello, world)

```C (Tells Markdown that code is in C)
printf("Hello, world\n");
```

All printed words are called strings and strings are enclosed by "string" <br>
\n tells computer to start a new line <br>
Most lines in C have to end in a ; (like period at the end of a sentence)

Scratch: Set counter to 0

```C
int counter = 0;
```

In C, you must declare the type of variable you are creating

Scratch: Change counter by 1

```C
counter = counter + 1; #Adds any number
counter + = 1; #Adds any number
counter + +; #only adds one
```

= doesn't mean equal in Comp-Sci, but it means assignment, Psuedo "Get" <br>
Don't need to say "int" for counter again because it was previously established

Scratch: If x < y     Say "x is less than y"

```C
if (x < y)
{
Printf("x is less than y \n");
}
```

Scratch: If x < y   Say "x is less than y"   else   Say "x is not less than y"

```C
if (x < y)
{
Printf("x is less than y \n");
}
Else
{
Printf("x is not less than y \n");
}
```

Scratch: Add another Else to previous statement

```C
if (x < y)
{
Printf("x is less than y \n");
}
Else if (x > y)
{
Printf("x is greater than y \n");
}
Else if (x == y)
{
Printf("x is equal to y n\");
}
```

== is actually equal to, while = is just assignments

Scratch: Forever saying Hello, world

```C
While(true)
{
Printf("hello, world \n");
}
```

Scratch: Say 50 time, Hello, world

```C
for (int i = 0; i < 50; i++)
{
printf("Hello, world \n");
}
```

Scratch: Ask "What is your name" and wait, say (answer)

```C
string answer = get_string("whats your name \n");
printf("%s", answer);
```

# Day 2

**cs50 IDE**

Directories = Folder

mkdir = Make directory

CD = change directory

CD .. = Go up one

LS = List everything

mv = move

mv (old file name) (new file name) = Change file name

rm = remove a file

rmdir = Remove Directory

**C Notes**

```C
#include <stdio.h>

int main(void)
{
printf("Hello, world\n");
}
```

./FILENAME = run file

# Day 3

You can add <cs.50.h>

```c
int main(void)
{
  string name = get_string("What is your name \n");
  Printf("Hello, %s\n", name);
}
```

get_int and get_string can be used to get integers and strings

% can be used to put in integers

```c
Include studios

int main(void)
{
  float x = get_float("x: ")
  
  float y = get_float("y: ")
}
```

%f
%f.2

```c
printf("x + y = %i \n")
```

Finite memory storing infinite numbers    NOT POSSIBLE

```c
int n = ("n: ");

if (n % 2 == 0)
{
printf("even\n")
}
else
{
printf("odd\n")
}
```

```c
int x = get_int("x: ");

int y = get_int("y: ");

if(x < y)
{
printf("x is less than y\n");
}
else if (x > y)
{
printf("x is greater than y\n");
}
```

1:40:58 on lecture 1

|| is or
& is and
! is not equal

# Day 4

Copy and paste is bad code

```c
#include <cs50.h>
#include <stdio.h>

int main(void)

{
    for (int i = 0; i < 3; i++)
        
    printf("cough\n");
}
```

Prototype: Put it at the beginning for C to find later in the code

do - while loops ensure the loop command is executed at least 1 time

##SUPER USEFUL TOOLS
help50
style50
check50
submit50

## Lecture 2

preprocessor
compiler - human words to computer words
assembly code - taking human words and translating it to computer acceptable words
machine code - turning computer words into 0s and 1s

Array - contiguous "Chunk" of memory for storing information i.e. char is 1 but int is 4

[ ] is used to say, "I have one variable, but want x amount of unique values"

Use 43:00 on cs50 lecture 2 video for help on arrays

int score[3]
  get 3 scores [][][]
  score is a variable, but you want 3 seperate answers
  
"global" variable
  const int COUNT = 3;   <---- This can help avoid putting 3, 3, 3, 3 making it easier to change into a new value / usually written in all caps to show a universal variable
  int score[count]
  
const- can't change this variable/ helps remove human error

combine string and array and use this to check the length of the string

use 55:00 for the string and array use

It is bad practice to put function in loop initialization

String = "Candy"
string[0] = "C"
s[1]=a
s[2]=n
so on
int c =(int)s[i]
Strings are arrays

A 5 letter word will be a 6 character array, \0 is used as the null character to signify the end

Casting: changing a data type

library ctype.h can use islower and toupper

man (manual) will help knowing how to use things
RTFM - Read The 'Flipping' Manual

argc: arguement count <---------------------- <br>
argv: arguement vector <----/                \ <br>
                                              | <br>
cs50 lecture 2 at 1:20:00 can help with above ^ <br>

string x = argv[0] //This is always going to be the program name, the first thing you gave

You cannot cast a string to an int

Cannot printf("%a", array)
must print it in a for loop using the elements
```c
for(int i = 0; i < n; i++);
{
  printf("%i", array[i])
}
```

for unique.c <br>
input 67275 <br>
should be 6725 <br>
myarray[6][7][2][7][5] <----- i <br>
unique array[6][7][2][5][X] <---- j <br>
int counter = 0 <br>

```c
for(int i = 0, ihiuwhiuhg)
{
  int counter = 0
  myarray[i]
  for(int j = counter jfhfuqhfu)
  {
  if(myarray[i]==unique[j])
  
  if not equal
  {
  unique[j]=myarray[i]
  counter++
```

for sort.c <br>
input 1362 <br>
output 1236 or 6321 <br>
myarray[1][3][6][2] <br>
sort[1][2][3][6] <br>

```c
for (int i = o; i < n; i++)
{
  for (int j = i + 1; j < n; j++)
  {
    if (myarray[i] > myarray[j])
    {
      myarray[1]=myarray[3]
      a = myarray[1]
      myarray[3] = a
```

make distinct error messages for argc argv code (areas.c)

1:25:00 on Lecture 2 for encrypted code

Plain text: Original text "I Love You"<br>
Ciphertext: Encode/ Encrypted text "J Knud Xnt"<br>
Key: "Secret" to decrypting or encrypting ciphertext; Each letter back one in alphabet<br>
Frequency attack: Guess & check based on how frequent words/letters are used; One may see the lone 'J' and assume 'A' or 'I', 'n' shows up twice, soon one may pick up this pattern

echo $? - can show the return values of main; This is useful because you can add "return (none zero number)" and do this to see where the error is/ where it is not working <br>
Return = 0: ALL GOOD! <br>
Return != 0: NOT GOOD!

SORTING METHODS

"Bubble" Sort <br>
Repeat until no swaps <br>
  for i from 0 to n-2 <br>
    if i'th and i+1'th elements out of order <br>
      swap them <br>
Pushes large values to the end to avoid looping all the way to the end all the time
      
"Selection" Sort <br>
for i from 0 to n-1 <br>
  find smallest element between i'th and n-1'th <br>
  swap smallest with i'th element <br>
Grabs the smallest element and replaces the i'th element

O(n) - Big Oh notation <br>
O(n) linear complexity <br>
O(n^2) Quadratic complexity <br>
O(log(n)) Logarithmic complexity <br>
O(n log(n)) Logarithmic linear <br>
O(1) Constant complexity <br>

TIME TAKEN : O(1) < O(log n) < O(n) < O(n log n) < O(n^2)
