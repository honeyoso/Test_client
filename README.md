# Test_client

Copy of work so far

import requests


#comment
#things to do on my machine: pip3, mkvirtualenv
#set up github repo
#in Pycharm: defined project
#response is a variable. We are assigning the value of "requests" is now the variable "Response". Value is what this returns.

response = requests.get('https://google.com')
print(response.content)

def add(a,b):
    return a + b
template = "3 + 4 = {}"
result = add(3,4)
print(template.format(result))
print( add(3,4))

#functions: they are just a block of code with a name. THey can either return a value or they can do things inside of the file/program/module.
#functions: don't necessarily have a return value. sometimes they just do shit.
#paramters: will change how the function behaves. Values that pass in to function and what the function operates on.
#return value: the thing that that function will return.
#invoke/call mean the same thing. It means execute the code with these parameters.

def getdata():
    server_url = 'https://google.com'
    response = requests.get(server_url)
    if response.status_code == 200:
        print(response)
    else: print('something bad happened')


getdata()

