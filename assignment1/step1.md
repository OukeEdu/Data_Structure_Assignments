First, we will get down the basic structure of the user interface. The grid of bacteria in your program gets its initial state from one of a set of provided input text files, which follow a particular format. When your program reads the grid file, you should re-prompt the user if the file specified does not exist. If it does exist, you may assume that all of its contents are valid. You do **NOT** need to write any code to handle a misformatted file. The behavior of your program in such a case is not defined in this spec; it can crash, it can terminate, etc. You may also assume that the input file name typed by the user does not contain any spaces. Make sure to close your input file streams when you are done reading the given file.

In each input file, the first two lines will contain integers r and c representing the number of rows and columns in the grid, respectively. The next lines of the file will contain the grid itself, a set of characters of size **row x column** with a line break (\n) after each row. Each grid character will be either a &#39;-&#39; (minus sign) for an empty dead cell, or an &#39;X&#39; (uppercase X) for a living cell. The input file might contain additional lines of information after the grid lines, such as comments by its author or even junk/garbage data; any such content should be ignored by your program.

The input files will exist in the same working directory as your program. For example, the following text might be the contents of a file simple.txt, a 5x9 grid with 3 initially live cells (the arrow notes are not part of the actual file):

_5 ←_ _number of rows tall_
_9 ←_ _number of columns wide_

_---------
--------- ←_ _- is a dead cell_

_---XXX--- ←_ _X is a living cell_

_---------
---------_

After your program reads the input file, you can print that file&#39;s lines to the console to test that your code works. Once this works, try reading the individual grid cells and turning them into a **Grid** object. You can print the current **Grid**&#39;s state on the console using **toString()** method provided in the grid class to see if it has the right data in it. Use a simple test case, e.g. **simple.txt**.