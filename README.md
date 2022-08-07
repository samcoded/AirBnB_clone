## Table of Contents

-   [Description](#description)
-   [Environment](#environment)
-   [File Explanation](#file_explanation)
-   [Getting Started](#getting_started)
-   [Running the tests](#running_the_tests)
-   [Usage](#usage)
-   [Authors](#authors)

## Description <a name = "description"></a>

This is a Airbnb clone projects that will be build with the aim to learn and apply concepts of high level programming and software engineering in general. In this first phase a basic console was created using the Cmd Python module, to manage the objects of the whole project, being able to implement the methods create, show, update, all, and destroy to the existing classes and subclasses.

## Environment <a name = "environment"></a>

The console was developed in Ubuntu 20.04LTS using python3 (version 3.4.3).

Further information 📑 For further information on python version, and documentation visit python.org.

## File Explanation <a name = "file_explanation"></a>

-   AUTHORS Contains info about authors of the project
    base_model.py Defines BaseModel class (parent class), and methods
-   user.py Defines subclass User
-   amenity.py Defines subclass Amenity
-   city.py Defines subclass City
-   place.py Defines subclass Place
-   review.py Defines subclass Review
-   state.py Defines subclass State
-   file_storage.py Creates new instance of class, serializes and deserializes data
-   console.py creates object, retrieves object from file, does operations on objects, updates attributes of object and destroys object

-   test_base_model.py unittests for base_model
-   test_user.py unittests for user
-   test_amenity.py unittests for amenity
-   test_city.py unittests for city
-   test_place.py unittests for place
-   test_review.py unittests for review
-   test_state.py unittests for state
-   test_file_storage.pyunittests for file_storage
-   test_console.py unittests for console

## Getting Started <a name = "getting_started"></a>

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Python3

### Installing

Clone this repository

```
git clone git@github.com:Samuel-Makinde/AirBnB_clone.git
cd AirBnB_clone
./console.py
```

## Running the tests <a name = "running_the_tests"></a>

This project uses the python unittest model for automated tests

#### Run all unit tests

`python3 -m unittest discover tests`

#### Run a test from a specific file

`python3 -m unittest tests/test_models/test_base_model.py`

## Usage <a name="usage"></a>

You can run the schell (in an interactive or non-interactive mode) to manipulate your models.
You can start it from running the console.py file:

```
$ ./console.py
```

The following commands are supported:

### create:

Creates a new instance of BaseModel, saves it (to the JSON file) and prints the id.
Ex:

```
$ create User
```

### show:

Prints the string representation of an instance based on the class name and id.
Ex:

```
$ show User 1234-1234-1234.
```

### destroy:

Deletes an instance based on the class name and id (save the change into the JSON file).
Ex:

```
$ destroy User 1234-1234-1234.
```

### all:

Prints all string representation of all instances based or not on the class name.
Example to show all instances

```
$ all
```

Example to show all instances of BaseModel only

```
$ all User
```

### update:

Updates an instance based on the class name and id by adding or updating attribute (save the change into the JSON file).
Ex:

```
$ update User 1234-1234-1234 email "sam@alxse.com"
```

### quit:

Quit the shell

## Authors <a name = "authors"></a>

-   [@Samuel-Makinde](https://github.com/Samuel-Makinde) - Samuel Makinde
-   [@samcoded](https://github.com/samcoded) - Samuel Anozie
