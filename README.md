# PythonProgrammingLessonNotes

## Episode 1: Python Fundamentals

Calculator:
```3 + 5 * 4```
Output:
```23```

Use a variable:

```weight_kg = 60```

* include letters, digits, underscores
* cannot start with a digit
* are case sensitive

Types of data:
* integer number
* floating point number
* string

weight_kg = 60 is an integer
weight_kg = 60.3 is a floating point
Create a string use quotes
patient_id = '001
Using variables: ```weight_lb = 2.2 * weight_kg
add a prefix to patient identifier:
patient_id = 'inflam_' + patient_id

## Built-in Functions
```print```
```print(weight_lb)```
```print(patient_id)```

**Output:**
```
132.66
inflam_001
```

Notice the parenthesis - requied for a function

Multiple things  with print function:
```print(patient_id, 'weight in kilograms:', weight_kg)```
Call a function inside another function:
```python
print(type(60.3))
print(type(patient_id))
```

**Output:**
```output
<class 'float'>
<class 'str'>
```
Moreover, we can do arithmetic with variables right inside the print function:
```python
print('weight in pounds:', 2.2 * weight_kg)
```
```output
weight in pounds: 132.66
```
does not change value of weight_kg:
```python
print(weight_kg)
```
```output
60.3
```

assign a new value:
```python
weight_kig = 65.00
print('weight in kilograms is now:', weight_kg)
```

```output
weight in kilograms is now 65.0
```
