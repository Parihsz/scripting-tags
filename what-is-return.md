### Tag Name: What is return?
### Tag Command: return

Picture a waiter asking to take down your order. The waiter's job is to relay that information to the kitchen who will produce the meal and have it brought to your table. 

Placing an order
* You tell the waiter what you want is like calling a function with specific instructions.
* ```lua
  local function add(x, y)
  -- The function 'add' receives your 'order' (x and y).
  end
  ```


Returning the Result:
* After your meal is prepared, the waiter brings it back to you. This is what the return keyword does in a function.
* ```lua
  local function add(x, y)
     return x + y -- returns the sum of x and y 
  end
  ```

Using the Result:
* You receive and use your meal by storing it in a variable.
* ```lua
  local sum = add(5, 3)
  print(sum)  -- Outputs: 8
  ```
