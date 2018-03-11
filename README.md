# binary-mnist
The standard MNIST dataset, with 12 variations for lower dimensionality, fewer categories, and smaller data types, all stored as ```.npy```'s. For use with *really* tiny models.



The repository consists of 3 dimensionality subdirectories:

* Original dimensionality (28x28, ``` original_28x28```)
* 14x14 dimensionality (14x14, ``` 14x14```,  generated with max pooling.)
* 7x7 dimensionality (7x7, ``` 7x7```,  generated with max pooling.)



Each subdirectory contains 4 permutations:

* ```binary_digits_binary_pixels```
  * Only one and zero digits, with all pixel values either a 1 or 0, rounded pixel/255. 
* ``` binary_digits_all_pixels```
  * Only one and zero digits, original pixel values (0-255). 
* ``` all_digits_binary_pixels```
  - All digits 0-9, with all pixel values either a 1 or 0, rounded pixel/255. 
* ``` all_digits_all_pixels```
  - Normal MNIST



I made this for my own personal use, but feel free to use it. 

I created all possible combinations, so don't mind if some don't seem necessary. 

All of the values are stored as numpy  ```int16``` 16 bit integers for uniformity, but can be easily converted. 