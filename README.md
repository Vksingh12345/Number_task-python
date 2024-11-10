# Number_task-python
def is_prime(n):

    if n <= 1:

        return False

    for i in range(2, int(n**0.5) + 1):

      if n % i == 0:

       return False
    return True


def fact(n):
    fact=1
    for i in range(1,n+1):
        fact=fact*i

    return fact 


def recur_fibo(n):
   if n <= 1:
       return n
   else:
       return(recur_fibo(n-1) + recur_fibo(n-2))

nterms = 10

# check if the number of terms is valid
if nterms <= 0:
   print("Plese enter a positive integer")
else:
   print("Fibonacci sequence:")
   for i in range(nterms):
       print(recur_fibo(i))
    


# Driver Program

print(" prime not prime chack your number:",is_prime(5))
print("factorial in number:",fact(5))
print("Fibonacci series:",recur_fibo(9))

    
      

  
