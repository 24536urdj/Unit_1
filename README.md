# Crypto Wallet
# Criteria A : Planning 
![](https://images.cointelegraph.com/images/1200_aHR0cHM6Ly9zMy5jb2ludGVsZWdyYXBoLmNvbS91cGxvYWRzLzIwMjItMDYvNDAyYjUzZGMtN2YzNC00Y2I0LTg4ZDgtYmRiYjg5NmFjODRiLmpwZw==.jpg)  
![](https://github.com/24536urdj/Unit_1/blob/main/%20blue%20planning.png) 
![](https://github.com/24536urdj/Unit_1/blob/main/Screen%20Shot%202022-10-09%20at%2014.55.58.png)
# Criteria B : Design 
"System Diagram"
![](https://github.com/24536urdj/Unit_1/blob/main/Screen%20Shot%202022-10-09%20at%2014.59.53.png)
"Flow diagram"

# Criteria C: Development

## Login System
My client requires a system to protect the private data. I thought about using a login system to accomplish this requirement using a if condition and the open command to work with a csv file. More description of the code....
```.py
def simple_login(user:str, password:str)->bool:
    '''
    Simple authentication, needs fle user.csv
    :param user: string
    :param password: string
    :return: True/False if user is in database
    '''
    with open("user.csv") as file:
        database = file.readlines()
    output = False
    for line in database:
        line_cleaned = line.strip() #remove \n
        user_pass = line_cleaned.split(",")
        if user == user_pass[0] and password == user_pass[1]:
            output = True
            break

    return output


```
