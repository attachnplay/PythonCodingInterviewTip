# PythonCodingInterviewTip

## sort vs sorted  (https://docs.python.org/3/howto/sorting.html)

### sort
- list_data.sort() method
- modify the list in-place
- list_data.sort()
- reverse
  - list_data.sort(reverse=True)
- list_data.sort(key=lambda x: x[0]) --> e.g., list_data = [(1,"Boy", "Kim"), (3, "Boy", "Lee")]

### sorted
- sorted() built-in function
- build a new sorted list from the iterable
- sorted(list_data)
- reverse
  - sorted(list_data, reverse=True)  
```python
test = ['bbb', 'aa', 'cccccc']
# Reverse sort
print(sorted(test, reverse=True))
# Sort by length
print(sorted(test, key=lambda x: len(x)))
# Original data
print(test)
```
- custom comparison
  - 
  ```
  def compare(x, y):
    if x + y > y + x:
      return -1
    else:
      return 1
  sorted(list_data, key=cmp_to_key(compare))
  ```


### defaultdict
  - collections.defaultdict(int)
  - 

### map
  
  
