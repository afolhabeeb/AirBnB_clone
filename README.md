# 0x00. AirBnB clone - The console
**Creation of a command interpreter to manage the hbnb projects**
## <p align="center">![alt text](https://github.com/afolhabeeb/AirBnB_clone/blob/master/AirBnB.png?raw=true)</p>

## Project Description
This is the first step towards building your first full web application: the **AirBnB clone**. The aim of the project is to deploy a replica of the [Airbnb Website](https://www.airbnb.com/) using my server. The final version of this project will have:
- ```A command interpreter to manipulate data without a visual interface, like a shell (for development and debugging)```
- ```A website (front-end) with static and dynamic functionalities```
- ```A comprehensive database to manage the backend functionalities```
- ```An API that provides a communication interface between the front and backend of the system.```

## Goal of this project
- ```Creation of a new object (ex: a new "User" or a new "Place")```
- ```Retrieval of an object from a file storage, a database etc… ```
- ```Perform operations on objects (count, compute stats, etc…)```
- ```Update attributes of an object```
- ```Destroy an object```
- 
## The created objects
**The list of the objects (instances) that can be created are as follows:**
- BaseModel
- User
- City
- Amenity
- State
- Review
- Place

## Files and Directories
- ```models``` directory contains all classes used for the entire project. A class, called “model” in a OOP project is the representation of an object/instance.
- ```tests``` directory contains all unit tests.
- ```console.py``` file is the entry point of our command interpreter.
- ```models/base_model.py``` file is the base class of all our models. It contains common elements:
    - attributes: ```id```, ```created_at``` and ```updated_at```
    - methods: ```save()``` and ```to_json()```
- ```models/engine``` directory contains all storage classes (using the same prototype). For the moment I will have only one: ```file_storage.py```.

## Usage Examples
## Launching the console

$ ./console.py
(hbnb) 
## Creating a new object

(hbnb) create
** class name missing **
(hbnb) create User
670265eb-5982-489e-8b92-2dff054f0776
## Show an object

(hbnb) show User
** instance id missing **
(hbnb) show User 670265eb-5982-489e-8b92-2dff054f0776
[User] (670265eb-5982-489e-8b92-2dff054f0776) {'created_at': datetime.datetime(2020, 2, 19, 18, 8, 58, 458246), 'id': '670265eb-5982-489e-8b92-2dff054f0776', 'updated_at': datetime.datetime(2020, 2, 19, 18, 8, 58, 458261)}
## Update an object

(hbnb) all
["[User] (70f71c16-962b-48ad-9df8-9203fe23d612) {'created_at': datetime.datetime(2020, 2, 19, 18, 11, 32, 341144), 'id': '70f71c16-962b-48ad-9df8-9203fe23d612', 'updated_at': datetime.datetime(2020, 2, 19, 18, 11, 32, 341161)}"]
(hbnb) update
** class name missing **
(hbnb) update User
** instance id missing **
(hbnb) update User 70f71c16-962b-48ad-9df8-9203fe23d612
** attribute name missing **
(hbnb) update User 70f71c16-962b-48ad-9df8-9203fe23d612  Age "20"
(hbnb) all
["[User] (70f71c16-962b-48ad-9df8-9203fe23d612) {'Age': 20, 'created_at': datetime.datetime(2020, 2, 19, 18, 11, 32, 341144), 'id': '70f71c16-962b-48ad-9df8-9203fe23d612', 'updated_at': datetime.datetime(2020, 2, 19, 18, 13, 9, 937933)}"]
(hbnb)
## Remove an object

(hbnb) destroy
** class name missing **
(hbnb) destroy User
** instance id missing **
(hbnb) destroy User 670265eb-5982-489e-8b92-2dff054f0776
(hbnb)
# Authors
- Habeeb A. Ojedokun
