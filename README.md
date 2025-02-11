# ZeroDivisionError in Average Calculation

This repository demonstrates a potential `ZeroDivisionError` in a Python function that calculates the average of a list of numbers. The bug occurs when the input list is empty or contains only zeros.

## Bug Description

The `calculate_average` function handles empty lists correctly by returning 0. However, it doesn't explicitly check if all numbers are zero.  If the sum is zero and the length is greater than zero, it still leads to division by zero. 

## Solution

The solution includes an additional check to ensure the sum of the numbers is not zero before performing the division.