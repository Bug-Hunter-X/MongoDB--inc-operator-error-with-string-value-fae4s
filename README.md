# MongoDB $inc operator error with string value

This example demonstrates an error that can occur when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numeric field by a specified value.  However, if you attempt to increment a numeric field with a string value, you'll get an error. This repository provides the incorrect code and the correct solution.

## Bug Description
The bug arises from attempting to increment the `count` field using a string instead of a number with the `$inc` operator.  MongoDB expects a numeric value for incrementation.

## Solution
The solution involves ensuring that the value used with the `$inc` operator is a number.