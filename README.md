# SI-GuidedProject-9858-1648545095
Guided Learning Module-Applied Data Science
## Exercises

Answer the questions or complete the tasks outlined in bold below, use the specific method described if applicable.

** What is 7 to the power of 4?**

A=7**4
A


** Split this string:**

    s = "Hi there Sam!"
    
**into a list. **

txt = "Hi there sam!"
b=txt.split()
b

txt = "Hi there sam!"
c=txt.split()
c

** Given the variables:**

    planet = "Earth"
    diameter = 12742

** Use .format() to print the following string: **

    The diameter of Earth is 12742 kilometers.

planet = "Earth"
diameter = 12742
print("The diameter of {} is {} kilometer".format(planet,diameter))



** Given this nested list, use indexing to grab the word "hello" **

lst = [1,2,[3,4],[5,[100,200,['hello']],23,11],1,7]

lst = [1,2,[3,4],[5,[100,200,['hello']],23,11],1,7]
print(lst[3][1][2][0])

** Given this nest dictionary grab the word "hello". Be prepared, this will be annoying/tricky **

d = {'k1':[1,2,3,{'tricky':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}

d = {'k1':[1,2,3,{'tricky':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}
print(d['k1'][3]["tricky"][3]['target'][3])

** What is the main difference between a tuple and a list? **



** Create a function that grabs the email website domain from a string in the form: **

    user@domain.com
    
**So for example, passing "user@domain.com" would return: domain.com**

def domain(email):
    print("Your domain is: " + email.split('@')[-1])

email = input("Please enter your email ID correctly ")
domain(email)



** Create a basic function that returns True if the word 'dog' is contained in the input string. Don't worry about edge cases like a punctuation being attached to the word dog, but do account for capitalization. **

def findDog(st):
    if 'dog' in st.lower():
        print("True")
    else:
        print("False")

st = input("Please key a string: >")
findDog(st)



** Create a function that counts the number of times the word "dog" occurs in a string. Again ignore edge cases. **

string = input("Please enter your string: ")

def countdogs(string):
    count = 0
    for word in string.lower().split():
        if word == 'dog' or word == 'dogs':
            count = count + 1
            print(count)

countdogs(string)



### Final Problem
**You are driving a little too fast, and a police officer stops you. Write a function
  to return one of 3 possible results: "No ticket", "Small ticket", or "Big Ticket". 
  If your speed is 60 or less, the result is "No Ticket". If speed is between 61 
  and 80 inclusive, the result is "Small Ticket". If speed is 81 or more, the result is "Big    Ticket". Unless it is your birthday (encoded as a boolean value in the parameters of the function) -- on your birthday, your speed can be 5 higher in all 
  cases. **

def caught_speeding(speed, is_birthday):
    
    if is_birthday:
        speeding = speed - 5
    else:
        speeding = speed
    
    if speeding > 80:
        return 'Big Ticket'
    elif speeding > 60:
        return 'Small Ticket'
    else:
        return 'No Ticket'

caught_speeding(60,4)

caught_speeding(90,4)

# Great job!
