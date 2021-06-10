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

#10.1. Pattern:
n=int(input("enter the number:"))
for i in range (n+1):
    for j in range (i):
        print(i,end='')
    print('')
    
#10.2
n=int(input("enter the number:"))
for i in range(n):
    for j in range(n):
        print(max(i+1,j+1,n-i,n-j),end='')
    print()   
    
#10.3.
n=int(input("enter the number:"))
for i in range(0,n):
    for j in range(0,i+1):
        print('*', end='')
    print('\r')
    
#10.4.
n=int(input("Enter the number:"))
for i in range (n+1,0,-1):
    for j in range (0,i-1):
        print("*",end='')
    print('')
    
#10.5.
n=int(input("enter the number:"))
for i in range(n):
    for j in range(n):
        print('#',end='')
    print()

#11. Write a program that computes the value of a+aa+aaa+aaaa with a given digit as the value of a.
#Suppose the following input is supplied to the program:9, Then, the output should be: 9 + 99 + 999 + 9999 =  11106.
a = int(input("Enter the number:"))
n1 = int( "%s" % a )
n2 = int( "%s%s" % (a,a) )
n3 = int( "%s%s%s" % (a,a,a) )
n4 = int( "%s%s%s%s" % (a,a,a,a) )
print(n1+n2+n3+n4)

#12. Find the length of a string using loops (not len()).
input_str= str(input("enter the string:"))
count=0
for i in input_str:
    count=count+1
print("length of the string:",end='')
print(count)
 
#13. Write a program that accepts a sentence (string) and calculate the number of letters and digits. Example: ‘this is a test sentence number 389’ ==> letters = 25 and digits = 3.
str = input("enter the sentence:")
letter=digit=0
for ch in str:
    if ch.isdigit():
        digit=digit+1
    elif ch.isalpha():
        letter=letter+1
    else:
        pass
print("digit:",digit)
print("letter:",letter)

#14.  Write a program that accepts a string and outputs the string with all capital letters.
#Example: ‘hello’ ==> ‘HELLO’. (using loop)
string = input(" Enter your Own String : ")
string1 = ''
for i in range(len(string)):
    if(string[i] >= 'a' and string[i] <= 'z'):
        string1 = string1 + chr((ord(string[i]) - 32))
    else:
        string1 = string1 + string[i]
print("\nOriginal String in Lowercase  =  ", string)
print("The Given String in Uppercase =  ", string1)

#15. Write a program that accepts a sentence and calculate the number of upper case letters and lower case letters.
santence=input("enter the sentence:")
upper_case=lower_case=0
for ch in str:
    if ch.isupper():
        upper_case=upper_case+1
    elif ch.islower():
        lower_case=lower_case+1
    else:
        pass
print("Upper:", upper_case)
print("Lower:", lower_case)

#16. Write  a program that counts the occurrence of a character in a string.
#Example: ‘This is a test string.’ count of i = 3.
str= input("Enter the string:")
c= input("Entr the character:")
res=0
for i in range(len(str)) :
    if(str[i]==c):
        res+=1
print(res)    
    
#17. Write a program to find if a given string is a palindrome or not.
s= input("Enter the string:")
if s == s[::-1]:
    print("is a palindrome")
else:
    print("is not a palindrome")
    
#18. Write a program which accepts two strings s1 and s2 and checks if s2 is a substring of s1.
string=input("Enter string:")
sub_str=input("Enter word:")
if(string.find(sub_str)==-1):
      print("Substring not found in string!")
else:
      print("Substring in string!")
      
#19.Make a password validator with the following checks. 
#A website requires the users to input username and password to register. 
#Write a program to check the validity of password input by users.
import re
password = input("Enter a password: ")
if len(password) < 8:
    print("Make sure your password is at lest 8 letters")
elif re.search('[0-9]',password) is None:
    print("Make sure your password has a number in it")
elif re.search('[a-z]',password) is None: 
    print("Make sure your password has a capital letter in it")
else:
    print("Your password seems fine")
    
#20. s = "Hello how are you all". For this given string write a code such that it prints the vowels present in the string s 
# if any.  ex: "i", "a" etc.
vowels = ['a', 'e', 'i', 'o', 'u']
characters_input = input('Type a sentence: ')
input_list = list(characters_input)
vowels_list = []
for x in input_list:
    if x.lower() in vowels:
        vowels_list.append(x)
vowels_string = ''.join(vowels_list)
print(vowels_string)
