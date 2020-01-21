## Recover.c

jpegs start 0xff 0xd8 0xff 0xe_ <--0-f

Images on a memory card are stored one after another, you must see the bytes to determine when a new image is started <br>
A buffer is speaked about a lot, it is temporary space used to store information while you look through it

Must use fopen to open the JPEG files, be aware of the null <br>
once it is open you must look at the bytes to see the start of each image <br>
A byte is defined in bmp.h from whodunit

fread (Data/struct, size of something, number of something, pointer)
^ This buffer that is being read should be a byte, buffer[512]. The buffer should be one block which is 512 bytes at a time

to find a JPEG, you must look at just the first 4 spots because the first 3 are always the same

Make a counter to track the number of images being found

use sprintf to store the JPEG file 

fwrite (data, size, number, outptr)

End of file (eof) is less than 512 bytes

open card file <br>
repeat until end of card <br>
  { <br>
  read 512 bytes into buffer <br>
  start of new JPEG <br>
    yes... <br>
    no... <br>
  Already found a JPEG <br>
    yes... <br>
    no... <br>
  } <br>
Close previous files <br>
