# Functions-in-python
var1 = [1, 2, 3, 4]
var2 = True
# Print out type of var1
print( type( var1))
# Print out length of var1
print(len(var1))
# Convert var2 to an integer: out2
out2 = int(var2)

first = [11.25, 18.0, 20.0]
second = [10.75, 9.50]
# Paste together first and second: full
full = first + second
# Sort full in descending order: full_sorted
full_sorted = sorted(full, reverse=True)
# Print out full_sorted
print(full_sorted)

# string to experiment with: place
place = "poolhouse"
# Use upper() on place: place_up
place_up = place.upper()
# Print out place and place_up
print(place)
print(place_up)
# Print out the number of o's in place
print(place.count('o'))

# Create list areas
areas = [11.25, 18.0, 20.0, 10.75, 9.50]
# Use append twice to add poolhouse and garage size
areas.append(24.5)
areas.append(15.45)
# Print out areas
print(areas)
# Reverse the orders of the elements in areas
areas.reverse()
# Print out areas
print(areas)

# Dictionary are Methods
# Definition of dictionary
europe = {'spain':'madrid', 'france':'paris', 'germany':'berlin', 'norway':'oslo' }
# Print out the keys in europe
print(europe.keys())
# Print out value that belongs to key 'norway'
print(europe['norway'])
# Add italy to europe
europe['italy'] = 'rome'
# Print out italy in europe
print('italy' in europe)

# Dictionary of dictionaries
europe = { 'spain': { 'capital':'madrid', 'population':46.77 },
           'france': { 'capital':'paris', 'population':66.03 },
           'germany': { 'capital':'berlin', 'population':80.62 },
           'norway': { 'capital':'oslo', 'population':5.084 } }

# Print out the capital of France
print(europe['france']['capital'])
# Create sub-dictionary data
data = { 'capital':'rome', 'population':59.83}
# Add data to europe under key 'italy'
europe['italy'] = data
# Print europe
print(europe)

# For loop
# areas list
areas = [11.25, 18.0, 20.0, 10.75, 9.50]
# Code the for loop
for ar in areas:
    print(ar)
# Change for loop to use enumerate() and update print()
for x, a in enumerate(areas) :
    print("room " + str(x) + ": " + str(a))
    
# Definition of dictionary
europe = {'spain':'madrid', 'france':'paris', 'germany':'berlin',
          'norway':'oslo', 'italy':'rome', 'poland':'warsaw', 'austria':'vienna' }
# Iterate over europe
for x, y in europe.items() :
    print("the capital of " + str(x) + " is " + str(y))
    
# Import numpy as np
import numpy as np
# For loop over np_height
for x in np_height : 
    print(str(x) + " inches")
# For loop over np_baseball
for x in np.nditer(np_baseball) : 
    print(x)

# Import cars data
import pandas as pd
cars = pd.read_csv('cars.csv', index_col = 0)
# Adapt for loop
for lab, row in cars.iterrows() :
  print(lab + ": " + str(row["cars_per_cap"]))
# Code for loop that adds COUNTRY column
for lab, row in cars.iterrows() :
    cars.loc[lab, "COUNTRY"] = row["country"].upper()
# Print cars
print(cars)

# Create a string: team
team = "teen titans"
# Define change_team()
 def change_team():
    """Change the value of the global variable team."""
# Use team in global scope
   global team
# Change the value of team in global: team
   team = "justice league"
# Print team
print(team)
# Call change_team()
change_team()
# Print team
print(team)  

# Define echo
def echo(n):
   """Return the inner_echo function."""
# Define inner_echo
   def inner_echo(word1):
       """Concatenate n copies of word1."""
       echo_word = word1 * n
        return echo_word
# Return inner_echo
   return inner_echo
# Call echo: twice
twice = echo(2)
# Call echo: thrice
thrice = echo(3)
# Call twice() and thrice() then print
print(twice('hello'), thrice('hello'))

# Define echo_shout()
def echo_shout(word):
    """Change the value of a nonlocal variable"""
# Concatenate word with itself: echo_word
   echo_word = word + word
# Print echo_word
   print(echo_word)
# Define inner function shout()
   def shout():
       """Alter a variable in the enclosing scope"""    
# Use echo_word in nonlocal scope
 nonlocal echo_word
# Change echo_word to echo_word concatenated with '!!!'
   echo_word = echo_word + '!!!'
# Call function shout()
  shout()
# Print echo_word
   print(echo_word)
# Call function echo_shout() with argument 'hello'
echo_shout('hello')

# Define gibberish
def gibberish(*args):
    """Concatenate strings in *args together."""
# Initialize an empty string: hodgepodge
   hodgepodge = ''
# Concatenate the strings in args
   for word in args:
        hodgepodge += word
# Return hodgepodge
   return hodgepodge
# Call gibberish() with one string: one_word
one_word = gibberish('luke')
# Call gibberish() with five strings: many_words
many_words = gibberish("luke", "leia", "han", "obi", "darth")
# Print one_word and many_words
print(one_word)
print(many_words)

# Define report_status
def report_status(**kwargs):
    """Print out the status of a movie character."""
     print("\nBEGIN: REPORT\n")
# Iterate over the key-value pairs of kwargs
   for key, value in kwargs.items():
        # Print out the keys and values, separated by a colon ':'
        print(key + ": " + value)
  print("\nEND REPORT")
# First call to report_status()
report_status(name = "luke", affiliation = "jedi", status = "missing")
# Second call to report_status()
report_status(name="anakin", affiliation="sith lord", status="deceased")


