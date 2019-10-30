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
