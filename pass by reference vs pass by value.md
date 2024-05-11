Tag Name: Pass by Value vs Pass by Reference\
Tag Command: pass-by-vs-reference

In Luau, variables can be passed by value or by reference depending on their data type. 
* Pass by value:
  - Numbers and other primitive data types are passed by value. When you assign a number to another variable or pass it to a function, a copy of the value is created. Any changes made to the copy does not affect the original value.
* Pass by reference:
  - Tables, on the other hand are passed by reference. When you assign a table to another variable or pass it to a function, you're passing a referene to the original table in memory. So, changes made to the table through the new variable or function will directly affect the original table.

Indirect Change is when you are changing the variable and not the actual value, for example:
```lua
local coin = player.leaderstats.Coin.Value
print(coin) --> 0
coin = 5
print(coin) --> 5
print(player.leaderstats.Coin.Value) --> 0
```
In this case, you are overwriting the variable, not changing the value.

The proper way to do it is:
```lua
local coin = player.leaderstats.Coin
coin.Value = 5
print(player.leaderstats.Coin.Value) --> 5
