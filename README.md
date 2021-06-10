#Q2. Print all odd numbers and even numbers between 1 to 100.
for i in range(1,100): 
    if i%2==0 :
        print(i,end=' ')
    if i%2==1 :
        print(i,end=' ')
        (or)
n = 1 
while(n<=100): 
        if(n%2==0): 
            print (n, "is even.")
        else:
             print (n, "is odd.") 
        n=n+1        
        
#Q3.Write a program to check if a number is prime or not.
n=int(input("enter the numner:"))
if n>1 :
    for i in range(2, int(n/2)+1):
        if (n%i) == 0 :
            print("number is not prime, FALSE")
            break
        else :
            print("number is prime, TRUE")
  
#Q4. Write a program that asks the user for a number n and prints the sum of the numbers 1 to n such that only multiples of three or five are considered in the sum, e.g. 3, 5, 6, 9, 10, 12, 15 for n=
a=1
sum=0
n=int(input("enter 😊the number:"))
for i in range (a,n):
    sum=sum+i
    if(i%3==0 or i%5==0):
        print(i,end=" ")

#5. Write a program that asks the user for a number n and gives them the possibility to choose between computing the sum and computing the product of 1,…,n.
n=int(input("enter the numner😊:"))
c=input("product or sum😍:")
p=1
s=0
if(c=="product"):
    for i in range(1,n):
        p=p*i;
    print(p)
else:
    for i in range(1,n):
        s=s+i;
    print(s)

#6. Find the sum of all the multiples of 3 or 5 below 1000.
a=1
sum=0
#n=int(input("enter 😊the number:"))
for i in range (a,1000):
    sum=sum+i
    if(i%3==0 or i%5==0):
        print(i,end=" ")
        
#7.Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000 and 3200 (both included).

for i in range (2000,3201):
    sum=sum+i
    if(i%7==0 and i%5!=0):
        print(i,end=" ")   
        
#8. Find the difference between the sum of the squares of the first one hundred natural numbers and the square of the sum
a=0
b=0
for i in range(1,101):
    a=a+i**2;
for i in range(1,101):
    b=b+i;
print(a-b**2)

#9. Write a program which can compute the factorial of a given number.
num=int(input("enter the number:"))
factorial=1
for i in range(1,num + 1):
       factorial = factorial*i
print("The factorial of",num,"is",factorial)
