## Tag Name: Common Error Messages
## Tag Command: common-errors

* [Name] is not a valid member of object
  - Meaning: Trying to access a non-existent child within an object.
  - Solution: Use `WaitForChild` since the child may not have loaded yet. If issue persists, check explorer and/or use print debugging.

* Attempt to index nil with something
  - Meaning: Trying to access an index of a nil variable.
  - Solution: Ensure variable is assigned before accessing its index. Check for typos, use print debugging to ensure the var is assigned the expected value from its source.

* Attempt to perform arithmetic (arithmetic) on number and [type]
  - Meaning: Performing arithmetic on incompatible data types.
  - Solution: Use arithmetic operations only on compatible types (numbers, strings, or objects with arithmetic metamethods (__mul, __add...). Also applies  to ``Attempt to compare something < number`` and ``Attempt to concatenate a string with something``

* Argument [number] missing or nil
  - Meaning: Sending a nil argument to a function.
  - Solution: Verify argument definition and type.

* Unable to cast value to Object
  - Meaning: Value cannot be converted into expected object type.
  - Solution: Ensure data type matches expectation before sending.

* Expected ')' (to close '(' at column [number]), got eof
  - Meaning: Syntax error indicating missing or extra parentheses.
  - Solution: Check for underlined sections, ensure all parentheses are balanced.
