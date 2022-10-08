# Common Error with If Statements
Here is a common error when joining if statements using logical conditions `and` `or` `not`.

In this example, I am trying to ignore the capitalization of the name for saying hi to Dave with `or`.

```python
name = input("Name: ")
if name == "Dave" or "dave":
  print("Hi Dave")
```
The computer does not read the if statement in the same way a person does. The left side is saying "If the name is equal to Dave", but the computer reads the right side as saying "Does Dave exist?"

Here is how we fix this:

We need to restate the full question.

```python
name = input("Name: ")
if name == "Dave" or name == "dave":
  print("Hi Dave")
```
