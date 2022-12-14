# get_random_people &middot; ![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg) [![Generic badge](https://img.shields.io/badge/version-1.1.3-<COLOR>.svg)](https://shields.io/)
A python package that generates huge dataset of fake, but real looking data of a person, that can be used to practice data science tools such as pandas. Useful to create graphs, tables, etc.
# Installation

```
pip install get_random_people
```

## Examples

### To get single person, `get_person()`

```
from get_random_people import get_random_people

user = get_random_people()
user.get_person() # eg:{"firstname": "Harry", "lastname": "Potter", ...}
```

In the above example `get_random_people().get_person()` will return a dictionary that has all the information of a person.

### To get multiple person, `get_peoples([n])`

```
from get_random_people import get_peoples

users = get_random_people().get_peoples() 
hundered_users = get_random_people().get_peoples(100)
```

In the above example ```get_peoples()``` will return a list of **10** person by default, but if you pass any numbers in the parenthesis it will return the list of that numbers of people, eg ```get_peoples(100)``` will return list of **100** people

### To get the property of a person
```
user = get_random_people().get_person()

print(user["firstname"]) #eg: Harry
print(user["lastname"]) #eg: Potter
print(user["age"]) #eg: 33
print(user["nationality"]) #eg: England
```

### All the properties of a person
```
 id,
 firstname,
 lastname,
 dob,
 email,
 phone_number,
 address,
 gender,
 religion,
 age,
 skin_color,
 eye_color,
 hair_style,
 hair_color,
 is_married,
 highest_education,
 occupation,
 side_bussiness,
 annaul_income_USD,
 nationality,
 height_in_feet,
 weight_in_kg
```

### Functions

```
from get_random_people import get_random_people

get_random_people().get_highest_education() # returns a qualification
get_random_people().get_phone_number([n]) # returns a phone number with n number of get_random_people().digits, if nothing is passed 10 digit number will be returned
get_random_people().get_DOB(age) # returns a date of birth, must pass age as integer
get_random_people().get_nationality() # returns a country name

```

&copy; 2022 InternetWebSoftwares | Ata Shaikh | Nicholes Viktor

This repository is licensed under the MIT license
See License for details.