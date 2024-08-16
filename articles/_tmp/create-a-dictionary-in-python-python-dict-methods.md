---
title: Create a Dictionary in Python – Python Dict Methods
date: 2024-08-16T03:41:26.030Z
author: Dionysia Lemonaki
authorURL: https://www.freecodecamp.org/news/author/dionysialemonaki/
originalURL: https://www.freecodecamp.org/news/create-a-dictionary-in-python-python-dict-methods/
translator: ""
reviewer: ""
---

In this article, you will learn the basics of dictionaries in Python.

<!-- more -->

You will learn how to create dictionaries, access the elements inside them, and how to modify them depending on your needs.

You will also learn some of the most common built-in methods used on dictionaries.

Here is what we will cover:

1.  [Define a dictionary][1]
    1.  [Define an empty dictionary][2]
    2.  [Define a dictionary with items][3]
2.  [An overview of keys and values][4] 1.[Find the number of `key-value` pairs contained in a dictionary][5] 2.[View all `key-value` pairs][6] 3.[View all `keys`][7] 4.[View all `values`][8]
3.  [Access individual items][9]
4.  [Modify a dictionary][10]
    1.  [Add new items][11]
    2.  [Update items][12]
    3.  [Delete items][13]

## How to Create a Dictionary in Python

A dictionary in Python is made up of key-value pairs.

In the two sections that follow you will see two ways of creating a dictionary.

The first way is by using a set of curly braces, `{}`, and the second way is by using the built-in `dict()` function.

### How to Create An Empty Dictionary in Python

To create an empty dictionary, first create a variable name which will be the name of the dictionary.

Then, assign the variable to an empty set of curly braces, `{}`.

```
#create an empty dictionary
my_dictionary = {}

print(my_dictionary)

#to check the data type use the type() function
print(type(my_dictionary))

#output

#{}
#<class 'dict'>
```

Another way of creating an empty dictionary is to use the `dict()` function without passing any arguments.

It acts as a constructor and creates an empty dictionary:

```
#create an empty dictionary
my_dictionary = dict()

print(my_dictionary)

#to check the data type use the type() function
print(type(my_dictionary))

#output

#{}
#<class 'dict'>
```

### How to Create A Dictionary With Items in Python

To create a dictionary with items, you need to include _key-value_ pairs inside the curly braces.

The general syntax for this is the following:

```
dictionary_name = {key: value}
```

Let's break it down:

-   `dictionary_name` is the variable name. This is the name the dictionary will have.
-   `=` is the assignment operator that assigns the `key:value` pair to the `dictionary_name`.
-   You declare a dictionary with a set of curly braces, `{}`.
-   Inside the curly braces you have a key-value pair. Keys are separated from their associated values with colon, `:`.

Let's see an example of creating a dictionary with items:

```
#create a dictionary
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

print(my_information)

#check data type
print(type(my_information))

#output

#{'name': 'Dionysia', 'age': 28, 'location': 'Athens'}
#<class 'dict'>
```

In the example above, there is a sequence of elements within the curly braces.

Specifically, there are three key-value pairs: `'name': 'Dionysia'`, `'age': 28`, and `'location': 'Athens'`.

The keys are `name`, `age`, and `location`. Their associated values are `Dionysia`, `28`, and `Athens`, respectively.

When there are multiple key-value pairs in a dictionary, each key-value pair is separated from the next with a comma, `,`.

Let's see another example.

Say that you want to create a dictionary with items using the `dict()` function this time instead.

You would achieve this by using `dict()` and passing the curly braces with the sequence of key-value pairs enclosed in them as an argument to the function.

```
#create a dictionary with dict()
my_information = dict({'name': 'Dionysia' ,'age': 28,'location': 'Athens'})

print(my_information)

#check data type
print(type(my_information))

#output

#{'name': 'Dionysia', 'age': 28, 'location': 'Athens'}
#<class 'dict'>
```

It's worth mentioning the `fromkeys()` method, which is another way of creating a dictionary.

It takes a predefined sequence of items as an argument and returns a new dictionary with the items in the sequence set as the dictionary's specified keys.

You can _optionally_ set a value for all the keys, but by default the value for the keys will be `None`.

The general syntax for the method is the following:

```
dictionary_name = dict.fromkeys(sequence,value)
```

Let's see an example of creating a dictionary using `fromkeys()` without setting a value for all the keys:

```
#create sequence of strings
cities = ('Paris','Athens', 'Madrid')

#create the dictionary, `my_dictionary`, using the fromkeys() method
my_dictionary = dict.fromkeys(cities)

print(my_dictionary)

#{'Paris': None, 'Athens': None, 'Madrid': None}
```

Now let's see another example that sets a value that will be the same for all the keys in the dictionary:

```
#create a sequence of strings
cities = ('Paris','Athens', 'Madrid')

#create a single value
continent = 'Europe'

my_dictionary = dict.fromkeys(cities,continent)

print(my_dictionary)

#output

#{'Paris': 'Europe', 'Athens': 'Europe', 'Madrid': 'Europe'}
```

## An Overview of Keys and Values in Dictionaries in Python

Keys inside a Python dictionary can **only be of a type that is immutable**.

Immutable data types in Python are `integers`, `strings`, `tuples`, `floating point numbers`, and `Booleans`.

Dictionary keys **cannot** be of a type that is mutable, such as `sets`, `lists`, or `dictionaries`.

So, say you have the following dictionary:

```
my_dictionary = {True: "True",  1: 1,  1.1: 1.1, "one": 1, "languages": ["Python"]}

print(my_dictionary)

#output

#{True: 1, 1.1: 1.1, 'one': 1, 'languages': ['Python']}
```

The keys in the dictionary are `Boolean`, `integer`, `floating point number`, and `string` data types, which are all acceptable.

If you try to create a key which is of a mutable type you'll get an error - specifically the error will be a `TypeError`.

```
my_dictionary = {["Python"]: "languages"}

print(my_dictionary)

#output

#line 1, in <module>
#    my_dictionary = {["Python"]: "languages"}
#TypeError: unhashable type: 'list'
```

In the example above, I tried to create a key which was of `list` type (a mutable data type). This resulted in a `TypeError: unhashable type: 'list'` error.

When it comes to values inside a Python dictionary there are no restrictions. Values can be of any data type - that is they can be both of mutable and immutable types.

Another thing to note about the differences between keys and values in Python dictionaries, is the fact that keys are **unique**. This means that a key can only appear once in the dictionary, whereas there can be duplicate values.

### How to Find the Number of `key-value` Pairs Contained in a Dictionary in Python

The `len()` function returns the total length of the object that is passed as an argument.

When a dictionary is passed as an argument to the function, it returns the total number of key-value pairs enclosed in the dictionary.

This is how you calcualte the number of key-value pairs using `len()`:

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

print(len(my_information))

#output

#3
```

### How to View All `key-value` Pairs Contained in a Dictionary in Python

To view every key-value pair that is inside a dictionary, use the built-in `items()` method:

```
year_of_creation = {'Python': 1993, 'JavaScript': 1995, 'HTML': 1993}

print(year_of_creation.items())

#output

#dict_items([('Python', 1993), ('JavaScript', 1995), ('HTML', 1993)])
```

The `items()` method returns a list of tuples that contains the key-value pairs that are inside the dictionary.

### How to View All `keys` Contained in a Dictionary in Python

To see all of the keys that are inside a dictionary, use the built-in `keys()` method:

```
year_of_creation = {'Python': 1993, 'JavaScript': 1995, 'HTML': 1993}

print(year_of_creation.keys())

#output

#dict_keys(['Python', 'JavaScript', 'HTML'])
```

The `keys()` method returns a list that contains only the keys that are inside the dictionary.

### How to View All `values` Contained in a Dictionary in Python

To see all of the values that are inside a dictionary, use the built-in `values()` method:

```
year_of_creation = {'Python': 1993, 'JavaScript': 1995, 'HTML': 1993}

print(year_of_creation.values())

#output

#dict_values([1993, 1995, 1993])
```

The `values()` method returns a list that contains only the values that are inside the dictionary.

## How to Access Individual Items in A Dictionary in Python

When working with lists, you access list items by mentioning the list name and using square bracket notation. In the square brackets you specify the item's index number (or position).

You can't do exactly the same with dictionaries.

When working with dictionaries, you can't access an element by referencing its index number, since dictionaries contain key-value pairs.

Instead, you access the item by using the dictionary name and square bracket notation, but this time in the square brackets you specify a key.

Each key corresponds with a specific value, so you mention the key that is associated with the value you want to access.

The general syntax to do so is the following:

```
dictionary_name[key]
```

Let's look at the following example on how to access an item in a Python dictionary:

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

#access the value associated with the 'age' key
print(my_information['age'])

#output

#28
```

What happens though when you try to access a key that doesn't exist in the dictionary?

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

#try to access the value associated with the 'job' key
print(my_information['job'])

#output

#line 4, in <module>
#    print(my_information['job'])
#KeyError: 'job'
```

It results in a `KeyError` since there is no such key in the dictionary.

One way to avoid this from happening is to first search to see if the key is in the dictionary in the first place.

You do this by using the `in` keyword which returns a Boolean value. It returns `True` if the key is in the dictionary and `False` if it isn't.

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

#search for the 'job' key
print('job' in my_information)

#output

#False
```

Another way around this is to access items in the dictionary by using the `get()` method.

You pass the key you're looking for as an argument and `get()` returns the value that corresponds with that key.

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

#try to access the 'job' key using the get() method
print(my_information.get('job'))

#output

#None
```

As you notice, when you are searching for a key that does not exist, by default `get()` returns `None` instead of a `KeyError`.

If instead of showing that default `None` value you want to show a different message when a key does not exist, you can customise `get()` by providing a different value.

You do so by passing the new value as the second optional argument to the `get()` method:

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

#try to access the 'job' key using the get() method
print(my_information.get('job', 'This value does not exist'))

#output

#This value does not exist
```

Now when you are searching for a key and it is not contained in the dictionary, you will see the message `This value does not exist` appear on the console.

## How to Modify A Dictionary in Python

Dictionaries are _mutable_, which means they are changeable.

They can grow and shrink throughout the life of the program.

New items can be added, already existing items can be updated with new values, and items can be deleted.

### How to Add New Items to A Dictionary in Python

To add a key-value pair to a dictionary, use square bracket notation.

The general syntax to do so is the following:

```
dictionary_name[key] = value
```

First, specify the name of the dictionary. Then, in square brackets, create a key and assign it a value.

Say you are starting out with an empty dictionary:

```
my_dictionary = {}

print(my_dictionary)

#output

#{}
```

Here is how you would add a key-value pair to `my_dictionary`:

```
my_dictionary = {}

#add a key-value pair to the empty dictionary
my_dictionary['name'] = "John Doe"

#print dictionary
print(my_list)

#output

#{'name': 'John Doe'}
```

Here is how you would add another new key-value pair:

```
my_dictionary = {}

#add a key-value pair to the empty dictionary
my_dictionary['name'] = "John Doe"

# add another  key-value pair
my_dictionary['age'] = 34

#print dictionary
print(my_dictionary)

#output

#{'name': 'John Doe', 'age': 34}
```

Keep in mind that if the key you are trying to add already exists in that dictionary and you are assigning it a different value, the key will end up being updated.

Remember that keys need to be unique.

```
my_dictionary = {'name': "John Doe", 'age':34}

print(my_dictionary)

#try to create a an 'age' key and assign it a value
#the 'age' key already exists

my_dictionary['age'] = 46

#the value of 'age' will now be updated

print(my_dictionary)

#output

#{'name': 'John Doe', 'age': 34}
#{'name': 'John Doe', 'age': 46}
```

If you want to prevent changing the value of an already existing key by accident, you might want to check if the key you are trying to add is already in the dictionary.

You do this by using the `in` keyword as we discussed above:

```
my_dictionary = {'name': "John Doe", 'age':34}

#I want to add an `age` key. Before I do so, I check to see if it already exists
print('age' in my_dictionary)

#output

#True
```

### How to Update Items in A Dictionary in Python

Updating items in a dictionary works in a similar way to adding items to a dictionary.

When you know you want to update one existing key's value, use the following general syntax you saw in the previous section:

```
dictionary_name[existing_key] = new_value
```

```
my_dictionary = {'name': "John Doe", 'age':34}

my_dictionary['age'] = 46

print(my_dictionary)

#output

#{'name': 'John Doe', 'age': 46}
```

To update a dictionary, you can also use the built-in `update()` method.

This method is particularly helpful when you want to update more than one value inside a dictionary at the same time.

Say you want to update the `name` and `age` key in `my_dictionary`, and add a new key, `occupation`:

```
my_dictionary = {'name': "John Doe", 'age':34}

my_dictionary.update(name= 'Mike Green', age = 46, occupation = "software developer")

print(my_dictionary)

#output

#{'name': 'Mike Green', 'age': 46, 'occupation': 'software developer'}
```

The `update()` method takes a tuple of key-value pairs.

The keys that already existed were updated with the new values that were assigned, and a new key-value pair was added.

The `update()` method is also useful when you want to add the contents of one dictionary into another.

Say you have one dictionary, `numbers`, and a second dictionary, `more_numbers`.

If you want to merge the contents of `more_numbers` with the contents of `numbers`, use the `update()` method.

All the key-value pairs contained in `more_numbers` will be added to the end of the `numbers` dictionary.

```
numbers = {'one': 1, 'two': 2, 'three': 3}
more_numbers = {'four': 4, 'five': 5, 'six': 6}

#update 'numbers' dictionary
#you update it by adding the contents of another dictionary, 'more_numbers',
#to the end of it
numbers.update(more_numbers)

print(numbers)

#output

#{'one': 1, 'two': 2, 'three': 3, 'four': 4, 'five': 5, 'six': 6}
```

### How to Delete Items from A Dictionary in Python

One of the ways to delete a specific key and its associated value from a dictionary is by using the `del` keyword.

The syntax to do so is the following:

```
del dictionary_name[key]
```

For example, this is how you would delete the `location` key from the `my_information` dictionary:

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

del my_information['location']

print(my_information)

#output

#{'name': 'Dionysia', 'age': 28}
```

If you want to remove a key, but would also like to save that removed value, use the built-in `pop()` method.

The `pop()` method removes but also returns the key you specify. This way, you can store the removed value in a variable for later use or retrieval.

You pass the key you want to remove as an argument to the method.

Here is the general syntax to do that:

```
dictionary_name.pop(key)
```

To remove the `location` key from the example above, but this time using the `pop()` method and saving the value associated with the key to a variable, do the following:

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

city = my_information.pop('location')

print(my_information)
print(city)

#output

#{'name': 'Dionysia', 'age': 28}
#Athens
```

If you specify a key that does not exist in the dictionary you will get a `KeyError` error message:

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

my_information.pop('occupation')

print(my_information)

#output

#line 3, in <module>
#   my_information.pop('occupation')
#KeyError: 'occupation'
```

A way around this is to pass a second argument to the `pop()` method.

By including the second argument there would be no error. Instead, there would be a silent fail if the key didn't exist, and the dictionary would remain unchanged.

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

my_information.pop('occupation','Not found')

print(my_information)

#output

#{'name': 'Dionysia', 'age': 28, 'location': 'Athens'}
```

The `pop()` method removes a specific key and its associated value – but what if you only want to delete the **last** key-value pair from a dictionary?

For that, use the built-in `popitem()` method instead.

This is general syntax for the `popitem()` method:

```
dictionary_name.popitem()
```

The `popitem()` method takes no arguments, but removes and returns the last key-value pair from a dictionary.

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

popped_item = my_information.popitem()

print(my_information)
print(popped_item)

#output

#{'name': 'Dionysia', 'age': 28}
#('location', 'Athens')
```

Lastly, if you want to delete all key-value pairs from a dictionary, use the built-in `clear()` method.

```
my_information = {'name': 'Dionysia', 'age': 28, 'location': 'Athens'}

my_information.clear()

print(my_information)

#output

#{}
```

Using this method will leave you with an empty dictionary.

## Conclusion

And there you have it! You now know the basics of dictionaries in Python.

I hope you found this article useful.

To learn more about the Python programming language, check out freeCodeCamp's [Scientific Computing with Python Certification][14].

You'll start from the basics and learn in an interacitve and beginner-friendly way. You'll also build five projects at the end to put into practice and help reinforce what you've learned.

Thanks for reading and happy coding!

---

![Dionysia Lemonaki](https://cdn.hashnode.com/res/hashnode/image/upload/v1713284398578/Zpo5ssvLj.jpeg)

Read [more posts][15].

---

If this article was helpful, share it.

Learn to code for free. freeCodeCamp's open source curriculum has helped more than 40,000 people get jobs as developers. [Get started][16]

[1]: #define-intro
[2]: #define-empty
[3]: #define-items
[4]: #overview
[5]: #length
[6]: #key-value
[7]: #keys
[8]: #values
[9]: #access
[10]: #modify
[11]: #add
[12]: #update
[13]: #delete
[14]: https://www.freecodecamp.org/learn/scientific-computing-with-python/
[15]: /news/author/dionysialemonaki/
[16]: https://www.freecodecamp.org/learn/