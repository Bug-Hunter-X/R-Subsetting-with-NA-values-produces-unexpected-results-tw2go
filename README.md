# R Subsetting with NA Values
This example demonstrates an uncommon error in R related to subsetting data frames when the condition involves NA values.  The issue arises from how R handles logical indexing with NA values; a comparison involving NA always results in NA, which is treated as FALSE when used for subsetting.

The `bug.R` file contains the code that exhibits the problem, and `bugSolution.R` provides a solution using the `is.na()` function for better control over handling NA values.

This issue is subtle and can lead to unexpected behavior if not handled correctly. The solution shows how to explicitly account for NA values in the subsetting process, ensuring that data with NA values is treated according to specific needs.