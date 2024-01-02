## Execution Control

Execution control involves structures like `if/elif/else,loops,and exceptions` for controlling program flow.

## If/Elif/Else

### Example of if/elif/else

```
x = 10
if x > 5:
    print("x is greater than 5")
elif x == 5:
    print("x is 5")
else:
    print("x is less than 5")
```

## For Loops

### Example of for loop

```
for i in range(5):
    print(i)
```

## Continue, Break

### Example of continue and break

```
for i in range(10):
    if i == 3:
        continue
    if i == 7:
        break
    print(i)
```

## While Loops

### Example of while loop

```
count = 0
while count < 5:
    print(count)
    count += 1
```

## Handling Exceptions

### Example of handling exceptions

```
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Error: Division by zero")
```
