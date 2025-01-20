# Unexpected Behavior from Directly Modifying Instance Variables in Ruby

This repository demonstrates a potential issue in Ruby where directly modifying instance variables using `instance_variable_set` can lead to unexpected behavior and make code less maintainable.  The `bug.rb` file showcases the problem, while `bugSolution.rb` provides a better approach using accessor methods.

## Problem

Direct manipulation of instance variables bypasses any validation, constraints, or side effects implemented in accessor methods (getters and setters). This can lead to inconsistencies and makes debugging and maintaining code more difficult. 

## Solution

Always use accessor methods (getter and setter) to interact with instance variables. This helps in maintaining encapsulation and data integrity. Accessor methods provide a controlled way to interact with object's state.