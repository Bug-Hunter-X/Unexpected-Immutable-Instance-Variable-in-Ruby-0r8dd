# Ruby Instance Variable Immutability Bug

This repository demonstrates a common pitfall in Ruby where instance variables can behave unexpectedly when you don't define explicit setter methods.  The `bug.rb` file shows how assigning a new value to an instance variable doesn't change its value if there's no associated setter method.  The solution, in `bugSolution.rb`, shows how to correctly define the setter method to allow modification.

## How to reproduce the bug

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `ruby bug.rb`.
4. Observe that the value of the instance variable does not change after the attempted assignment.

## Solution

The solution involves defining an explicit setter method (e.g., `value=`).  This allows modifying the instance variable's value externally.