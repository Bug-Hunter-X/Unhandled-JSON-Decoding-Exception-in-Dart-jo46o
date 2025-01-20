# Unhandled JSON Decoding Exception in Dart

This repository demonstrates a common error in Dart: neglecting to properly handle exceptions that can occur during JSON decoding. The `bug.dart` file showcases code that fails to handle a `FormatException` that could occur if the JSON response from an API is invalid. The `bugSolution.dart` file provides a corrected version which utilizes a `try-catch` block to specifically handle `FormatException`, enabling more robust error management.

## How to Reproduce

1. Clone this repository.
2. Run `bug.dart`. Observe that, if the API request fails to return valid JSON, a generic error message is printed.
3. Run `bugSolution.dart`. The improved error handling provides a more informative message about the JSON decoding failure.

## Solution

The solution involves a `try-catch` block within the `fetchData` function, specifically catching the `FormatException` which occurs during JSON decoding.  This allows for more refined error handling and more informative error messages, making debugging easier.
