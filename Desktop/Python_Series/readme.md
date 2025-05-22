#Create a function that takes no arguments and prints "hello world"

def function():
    print("hello world")
function()    


#write a function to calulate and rreturn sun of two numbers
def function1 (a,b):
    z=a+b 
    #print(z)
    return z
   
# result=function1(5,6)
# print(result)
print(function1(5,7))


#create a function that return both area and circumference of a circle
#given its radius

def circle_stas(radius):
    area=3.14*radius*radius
    circumference=2*3.14*radius
    return area,circumference
result=circle_stas(5)
print(result)


#write a function tthat greet a user if no name is provided it 
#should greet with default name  
def greeting(name="khageswar"):
    print(f"hello,{name}")
greeting()
greeting("john")

#lambda function
cube=lambda x: x**3
print(cube(3))


#Write a function that takes variable number of arguments
#  retun their sum

def sum_all(*args):
    print(args)
    return sum(args)
print(sum_all(1,2,3))
print(sum_all(1,2,3,4,5))
print(sum_all(1,2,3,4,5,6,7,8,9,10))     



# create a functionthat accept any number of keyword arguments
# and printthem in the form of key=value

def print_kwargs(**kwargs):
    for key,value in kwargs.items():
        print(f"{key}={value}")
print_kwargs(name="khageswar",age=25,city="kathmandu")
print_kwargs(name="john",age=30,city="newyork",country="USA")
print_kwargs(name="sita",age=22,city="delhi",country="india",hobby="reading")




# create a recursive function to calculate the factorial of a number

def factorial(n):
    if n==0 or n==1:
        return 1
    else:
        return n*factorial(n-1)
print(factorial(5))    