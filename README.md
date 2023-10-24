# pyscript_filesizes
This is a Python script I built as part of a course that will traverse the filesystem finding the largest files in a path.

## 1. Import OS
This is the module which allows you to interact with your operating system and thus will give you the ability to traverse the file
system.

## 2. meta_data dictionary
This second block of code, creates a persistent dictionary which will store the metadata of the files such as their name and size.

## 3. I have set 3x variables
- items_presented - This acts as a counter starting from 0 for the for loop.
- min_size_b - This is a size parameter (bytes) that will allow you to filter results.
- max_files - This is another parameter, only this one allows you to filter the maximum amount of files for the return.

## 4. selected_files
This creates an empty tuple for the results to be appended

## 5. The for loop

### The first part of the for loop 
grabs the filepath and size, and sorts them by size in reverse order

### The second part of the loop 
says if items_presented (initially set to 0) is more or equal to our max_files parameter of 20 then break.

### The third part of the loop 
adds another if statement to allow our minimum size (bytes) to also be captured here.

### The fourth part of the loop 
appends the paths and sizes identified with the loop, to the empty tuple created previously.

### The last part of the loop 
increases the counter of the items_presented variable, and will continue to increase until the second part of the loop = True in which case the break function will be envoked and the loop will end.

## 6. The results
This is another simple for loop which will print all the selected files from the tuple in a nice readable format that also converts the bytes to MB and displays the path separated by hyphen.

I hope you enjoyed this reading, feel free to fork and modify this code as you so choose.
