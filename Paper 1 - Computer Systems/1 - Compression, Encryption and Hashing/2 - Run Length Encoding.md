
## Dictionary Coding

- This is a method of lossless compression that uses dictionaries, like the data structure used in programming
- Each value has a key value related to it, meaning you can use simple values to reference to much more complex words.
- The main thing that takes up the storage is the dictionary itself, as it needs to assign each value, but this will be more efficient than repeating longer references.
- This is very efficient on text, but not applicable on images


## Run Length Encoding

- This is used on bitmap images, and isn't ideal for text
- The issue with bitmap is that it is made up of several discrete pixels, which is very hard to recreate.
- The way we compress this, is by looking at each pixel, and saying how many of the same one there is in a row, e.g. 22 white, followed by 6 black, followed by 31 white etc. 
- This is stored in what we call frequency pairs
	- 22 0 tells us there are 22 contiguous black pixels
	- 12 1 tells us there are 11 contiguous white pixels