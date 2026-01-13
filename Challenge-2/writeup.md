#challenge-2
Task: 1. Analyze the image
      2. Extract hidden information

Hint: Use the command to view and analyze binary files in hexadecimal format.

Analysis:
1. Convert the JPEG file to a binary file. (cp image.jpg image.bin)
2. Convert the binary file to a text file with hexadecimal view. (xxd image.bin > image.hex)
    ~xxd: converts binary file to hex dump
3. Search "flag" in this text file. (grep "flag" image.hex). 
    ~ This command would show the line in the hex view where "flag" is found.
    This command only gave me partial output. 
4. Retrieve full output. (grep -C 1 "flag" image.hex )
    ~grep: searches text
    ~-C 1: to show 1 line before and after the searched text.
Flag: flag{jai_mahismathi}
