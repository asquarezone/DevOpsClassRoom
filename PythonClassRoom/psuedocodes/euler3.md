# Euler Problem 3

The prime factors of 13195 are 5, 7, 13 and 29.

What is the largest prime factor of the number 600851475143 ?

## Psuedo Code

function isPrime: number returns boolean
isPrime = true
repeat index from 2 till number-1
  if number %  index  equals 0
     isPrime = false
     return isPrime
  end if 
  index = index + 1
end repeat
return isPrime
end function

function largestFactor: input 

repeat index from number/2 till 2
if number % index == 0
    if isPrime(index)
       print result is index
     end if
end if
index = index -1
end repeat
end function

