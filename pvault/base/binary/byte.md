#unit
A collection of 8 [[bit]]s, similar to a kilogram in unit representation. Why 8? "Its just more useful, as well as being a power of 2".


It does help to know the lower and higher bounds of each digit type, as you can pre-emptively think of how much [[Memory]] you want to allocate.

e.g. :
```
128  64  32  16  8  4  2  1
#    #   #   #   #  #  #  # 
0    0   0   0   0  0  0  0  = 0
---
128  64  32  16  8  4  2  1
#    #   #   #   #  #  #  # 
1    1   1   1   1  1  1  1  = 255 + 0 (256 total)
```