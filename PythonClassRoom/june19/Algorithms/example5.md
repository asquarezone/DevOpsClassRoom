## Find the reverse of number
1. allocate memory locations for __number__ = 356, __reverse__=0 
2. repeat till number is  not zero
3. allocate memory for __lastdigit__ 
4. __lastdigit__ = __number__ %10
5. __number__ = __number__ /10
6. __reverse__ = __lastdigit__ + (__reverse__*10)
7. go to step 3
8. print __reverse__


)356(35
   350
--------
      6

10)35(3

------
  5

  6*10+5 = 65

10)3(0
-----
3

65*10+3