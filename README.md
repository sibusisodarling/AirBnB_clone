# AirBnb clone - The console

* How to create a Python package
* How to create a command interpreter in Python using the cmd module
* What is Unit testing and how to implement it in a large project
* How to serialize and deserialize a Class
* How to write and read a JSON file
* How to manage datetime
* What is an UUID
* What is *args and how to use it
* What is **kwargs and how to use it
* How to handle named arguments in a function

## Examples

EXAMPLE:

The input: program that contains the entry point of the command interpreter:

The output:

```
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) help quit
Quit command to exit the program

(hbnb) 
(hbnb) 
(hbnb) quit
```

### Non-Interactive Mode

$ echo "help" | ./console.py
(hbnb)
Documented commands (type help <topic>):
========================================
EOF  all  count  create  destroy  help  quit  show  update

(hbnb) $
$
$ echo "create BaseModel" | ./console.py
(hbnb) f09bfbad-532d-4bbe-a2c1-815b1958f01e
(hbnb) $
$ echo "all" | ./console.py
(hbnb) [[BaseModel] (f09bfbad-532d-4bbe-a2c1-815b1958f01e) {'id': 'f09bfbad-532d-4bbe-a2c1-815b1958f01e', 'updated_at': datetime.datetime(2024, 5, 18, 23, 16, 30, 420332), 'created_at': datetime.datetime(2024, 5, 18, 23, 16, 30, 420300)}]
(hbnb) $
$ echo "destroy BaseModel f09bfbad-532d-4bbe-a2c1-815b1958f01e" | ./console.py
(hbnb) (hbnb) $
$ echo "all" | ./console.py
(hbnb) []
(hbnb) $
$
