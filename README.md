# MongoDB $inc Operator Error: Non-numeric Increment Value

This example demonstrates an uncommon error in MongoDB update operations involving the `$inc` operator. The `$inc` operator is used to increment a numerical field by a specified value. However, providing a non-numeric value as the increment results in an error.

## Bug Report

The bug lies in the incorrect usage of the `$inc` operator. Attempting to increment the `count` field with a non-numeric value ('abc') causes the update operation to fail.

## Solution

To fix this, ensure that the value passed to the `$inc` operator is a valid number.  The updated code corrects this issue.