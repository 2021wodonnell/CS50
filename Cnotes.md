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

