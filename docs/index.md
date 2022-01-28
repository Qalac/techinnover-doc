# Techinnover Technical Test

This documentation is aimed to help setup and better understand the project.

## Installation

This project is completely written in python so you'll need python setup tools like pip, venv and a python intepreter. You are advised to make use of a python virtual environment as it is good practice. If you're unfamiliar with these tools, click this link to better understand the setup [https://packaging.python.org/guides/installing-using-pip-and-virtual-environments]. Upon setting up these tools, you'll want to run the code below to copy the project source code to your local machine.

```bash
git clone https://github.com/Qalac/techinnover-test.git
```

## Project Startup

Upon successful cloning of the repository, navigate to the root directory and run the following code below to run the source code.
```bash
python3 index.py
```

## Testing

To carry out unit testing, run the following code below to run all the unit tests associated with this project
```bash
python3 -m unittest discover -s tests
```

## Structure

The project is divided into modules to allow scaling and extensive improvement with time. The file structure is represented below

```
project
│ 
│   README.md
│   index.py    
│
└────── Plateau/
│       __init__.py
│       plateau.py
│ 
│────── Rover/ 
│       __init__.py
│       rover.py
│ 
│────── middleware/    
│      __init__.py
│      middleware.py
│ 
│────── tests/        
       __init__.py
       test_middleware.py
       test_plateau.py
       test_rover.py

```

## Test Cases

The table below shows the various test cases and the required outcomes

| No.|           Test                          | Expected result |
| :--|          :----:                         |     ---:        |
| 1  | test_rover_is_not_within_perimeter      | Pass            |
| 2  | test_rover_is_within_perimeter          | Fail            |
| 3  | test_rover_x_is_not_within_perimeter    | Pass            |
| 4  | test_rover_x_is_within_perimeter        | Fail            |
| 5  | test_rover_x_is_landing_on_rover        | Pass            |
| 6  | test_rover_x_is_not_landing_on_rover    | Fail            |
| 7  | test_rover_is_making_invalid_movements  | Pass            |
| 8  | test_rover_is_making_valid_movements    | Fail            |
| 9  | test_rover_x_is_making_invalid_movement | Pass            |
| 10 | test_rover_x_is_making_valid_movement   | Fail            |
| 11 | test_plateau_creation                   | Pass            |
| 12 | test_rover_creation                      | Pass            |
| 13 | test_setLeft_function                   | Pass            |
| 14 | test_setRight_function                  | Pass            |
| 15 | test_moveForward_function               | Pass            |


