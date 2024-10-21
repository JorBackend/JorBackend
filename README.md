# About Jonathan Baker
<img src = "https://media.licdn.com/dms/image/v2/D5603AQHs0hKqKgP-Jw/profile-displayphoto-shrink_200_200/profile-displayphoto-shrink_200_200/0/1719783800192?e=1735171200&v=beta&t=wXPsLKBAqQlwl6x6FIL8MzijRx5kW-tyuCzKuPd5Tlk">

<a href="https://www.linkedin.com/in/jonathanr-baker/"><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRokEYt0yyh6uNDKL8uksVLlhZ35laKNQgZ9g&s" width = 50px href="https://www.linkedin.com/in/jonathanr-baker/"></a>
<a href = "https://github.com/JorBackend"><img src="https://github.githubassets.com/assets/GitHub-Mark-ea2971cee799.png" width=50px></a>

<b>I am 17 years old and I go to Castle High School and SICTC</b>

<b>I will be attending the University of Evansville in Fall 2026</b>
## Projects
### LunchBox Data Collector
- Android Studio app developed to hold order data at SICTC's LunchBox
- App developed with Java and XML in order to send data to a MySql database
- Data stored on Raspberry Pi
- Flask website with Login for Chef to see important data

### Animal Quiz
- Website created for Vet Science program at SICTC to help students study animal parts
- Game created using Trinket & embedded on website
- Hosted on GitPages

## Work Experience
- The Fresh Market
  - August 2024 - Present
  - Maintain positive attitude with customers
  - Provide great customer service
  - Get customers through as quickly as possible

- Boomerang Learning
  - July 2024 - Present
  - Manage and maintain databases hosted on Microsoft Azure
  - Feed user info into OpenAI to create and verify question on user’s lowest level
  - Maintain employees' responsibilities and verify code
 
- Nextech Catapult Internship
  - June 2024 - July2024
  - Communicate effectively with associates
  - Collaborate with associates to complete projects
  - Critically think to effectively complete assignments on time

## Programming Background
|Programming Languages|
|---|
|Python|
|SQL|
|Java|
|JS|
|C++|
|HTML|
|CSS|
|C#|
|VB|
<br>

|Classes|
|---|
|CS-210: Fundamentals of Programming I|
|CS 1|
|Computer Science Software Development|
|Nextech Catapult|
<br>

## Scripting Examples
### Account Updater for MySql DB
```python
### Upload accounts to basic MySql server hosted on raspberryPi at SICTC
import pandas as pd
file = pd.read_csv("Accounts.csv",header=0, encoding="utf-8")

### NEED TO CLEAN THE DATA AND BE SURE ALL FILES HAVE APPORIATE DATA

queries=""
for i in range(0,len(file)):
    try:
        queryString = f"""
INSERT INTO Accounts
(Names,Address,City,State,Zip,Phone)
VALUES("{file['name'][i]}",
    "{file['address'][i]}",
    "{file['city'][i]}",
    "{file['state'][i]}",
    "{file['zip'][i]}",
    "{file['phone'][i]}");"""
        queries+=queryString+"\n"
    except:
        print(i)
        
with open("AccountsUpload.sql","w+", encoding="utf-8") as file:
    file.write(queries)    
```

### 2D Player Controller
```vb
'px and py stand for the location of the player right before it is moving and udlr represent up, down, left, and right. Whenever they are true it is moving them whichever direction 2 pixels on the timer 
 px = pnlPlayer.Location.X
 py = pnlPlayer.Location.Y

        If u = True Then
            pnlPlayer.Location = New Point(pnlPlayer.Location.X, pnlPlayer.Location.Y - 2)
        End If

        If d = True Then
            pnlPlayer.Location = New Point(pnlPlayer.Location.X, pnlPlayer.Location.Y + 2)
        End If

        If l = True Then
            pnlPlayer.Location = New Point(pnlPlayer.Location.X - 2, pnlPlayer.Location.Y)
        End If

        If r = True Then
            pnlPlayer.Location = New Point(pnlPlayer.Location.X + 2, pnlPlayer.Location.Y)
        End If
```
