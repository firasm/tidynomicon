- Don't use `setwd`.
- The formula operator `~` delays evaluation of its operand or operands.
- `~` was created to allow users to pass formulas into functions, but is used more generally to delay evaluation.
- Some tidyverse functions define `.` to be the whole data, `.x` and `.y` to be the first and second arguments, and `..N` to be the N'th argument.
- These convenience parameters are primarily used when the data being passed to a pipelined function needs to go somewhere other than in the first parameter's slot.
- 'Copy-on-modify' means that data is aliased until something attempts to modify it, at which point it duplicated, so that data always appears to be unchanged.
