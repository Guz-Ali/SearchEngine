# SearchEngine
Find images through keywords with their tags, and display it.

## Required Libraries
os, glob, PIL, pickle.

To install libraries, do:
`pip install *library*`

If you do not have PIL or pickle, simply run this code on terminal: 
`pip install PIL pickle`

## Test Cases
I have three default test cases for the function `search_text(...)` 


## How to open the program
Run jupyter notebook Search-Image-Shopify-Project.ipynb on terminal while in directory, or open the file directly.

Please run all nodes. You can check the test cases.

I have left a playground for you to use the function `search_text` to search by keywords. You can change the keywords to try out the program.

## What my class and functions do
First the program loads the images (.png) and the tags (.pk). By now, we created the class, all that's left is to try the program out.

Program uses user's keywords to find the images through their tags.

Try these codes in the playground section:

To see the tags, you can run `engine.print_tags()`

To simply use the engine, use function `engine.search_text(["your","keys"])`. By default, program will display images that have the keys as their tags. (by default program uses operator "and").
  
  To run with operator "or" instead, do: `engine.search_text(["your","keys"], op="or")`
  
  To make the program display no images, do: `engine.search_text(["your","keys"], suppress_images="True")`
  
## Final notes
I used the Azure Computer Vision examples as my database but their API could be implemented directly to our program.
