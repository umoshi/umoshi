#system 
Binary/base-2,

Two possible states, ON or OFF. Most commonly seen in [[Computer Science]].

Counting in binary:

```
0 = 0
1 = 1
10 = 2
11 = 3
100 = 4
101 = 5
110 = 6
111 = 7
```
Each ON & OFF state per [[bit]] represents a different state entirely, such the new number, the more bits the higher you can count. 8 possibilities, 7 distinct numbers without counting 0.

Similarly to the decimal system this uses a power, this time of 2.

e.g.  with 3 bits :
```
2^2  2^1  2^0
#    #    # 
4    2    1
```

We can still fairly easily count if we weight the order appropriately by thinking of each slot as a number * the state of that number. We then add the value of each slot together with the previous.

e.g. :
``` S = slot | V = value
S 4   2   1  
V #   #   #  =  4*#  2*#  1*#

--- In use example ---
S 4   2   1
V 1   0   1  =  4*1  2*0  1*1  =   5
```

You can only count to 7 with 3 [[bit]]s, so you need more "[[Memory]]" per-se, to represent and manage more numbers.

An easy way to calculate bit slot weights in your head is :
$$
previous * 2
$$

Though singular bits aren't all too useful, so the standard unit of measurement when handling computer memory/storage is [[byte]]s.



## Representing letters
By taking the alphabet and assigning a value to each letter you can represent the alphabet in binary form! And such around 100 years ago it was decided in a room that  " A " would be represented by 01000001, who's value is 65. B being 66 and so on.