# 0x00. AirBnB clone - The console
**Creation of a command interpreter to manage the hbnb projects**
## <p align="center">![alt text](https://github.com/afolhabeeb/AirBnB_clone/blob/master/AirBnB.png?raw=true)</p>

## Description of the project
This is the first step towards building your first full web application: the **AirBnB clone**. The aim of the project is to deploy a replica of the [Airbnb Website](https://www.airbnb.com/) using my server. The final version of this project will have:
- ```A command interpreter to manipulate data without a visual interface, like a shell (for development and debugging)```
- ```A website (front-end) with static and dynamic functionalities```
- ```A comprehensive database to manage the backend functionalities```
- ```An API that provides a communication interface between the front and backend of the system.```

## Aims & Objectives of this project
**This will help to be able to manage the objects of our project:**
- ```Creation of a new object (ex: a new "User" or a new "Place")```
- ```Retrieval of an object from a file storage, a database etc… ```
- ```Perform operations on objects (count, compute stats, etc…)```
- ```Update attributes of an object```
- ```Destroy an object```
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

# Authors
- Habeeb A. Ojedokun
