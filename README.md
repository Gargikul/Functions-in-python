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

# Dictionary
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
