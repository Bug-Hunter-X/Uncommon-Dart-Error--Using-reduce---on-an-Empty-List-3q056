# Uncommon Dart Error: Using reduce() on an Empty List

This repository demonstrates an uncommon error in Dart that can occur when using the `reduce` method on an empty list. The `reduce` method requires at least one element in the list. If the list is empty, it throws a `StateError` exception.

The `bug.dart` file contains the code that produces the error. The `bugSolution.dart` file contains the corrected code that handles the case of an empty list.

## How to Reproduce

1. Clone this repository.
2. Run the `bug.dart` file using the Dart command line:
   ```bash
   dart bug.dart
   ```

You will see a `StateError` exception.

## Solution

The solution is to check if the list is empty before calling `reduce`. If the list is empty, you should return a default value or handle the empty case appropriately.  This is shown in `bugSolution.dart`.