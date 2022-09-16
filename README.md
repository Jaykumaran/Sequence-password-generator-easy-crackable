# Sequence-password-generator-easy-crackable

import random


small_letters=['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
capital_letters=['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
numbers=['0', '1', '2' , '3', '4','5','6','7','8','9']
symbols=['!', '@', '#', '$', '%' , '&', '*','(','~']
print("Welcome to PyPassword Generator")
no_of_small_letters=int(input(f"How many small letters would you like in your password? : \n "))
no_of_capital_letters=int(input(f"How many capital letters would you like in your password? : \n "))
no_of_symbols=int(input(f"how many symbols would you like? to have in passwords? :  \n"))

no_of_numbers=int(input(f"how many numbers would you like to have in pass? \n"))

#easy level
password=""
for char in range(1, no_of_capital_letters+1):

  password+= random.choice(capital_letters)
  
for char in range(1, no_of_small_letters+1):

  password+= random.choice(small_letters)
for char in range(1, no_of_numbers+1):

  password+= random.choice(numbers)
for char in range(1, no_of_symbols+1):

  password+= random.choice(symbols)
print(password)
  

output sample:
Welcome to PyPassword Generator
How many small letters would you like in your password? : 
 2
How many capital letters would you like in your password? : 
 3
how many symbols would you like? to have in passwords? :  
4
how many numbers would you like to have in pass? 
1
YBXyd3%(##
