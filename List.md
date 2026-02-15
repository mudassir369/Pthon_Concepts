# LIST

- List are used to stor multiple items in a single variable.
- List are created using square brackets.
- List items are ordered, changeable(mutable) and allow duplicate values.
- List items are indexed, the first item has index [0], the second item has [1] etc.
- A list can contain different data types.

### Example

```bash
thislist = ["apple","banana","cherry"]
list1 = ["Mohammad", 45, True, "Mudassir"]
```

## Most Important List Method 

### 1. append()

Add one element at the end

```bash
nums = [1,3,2]
nums.append(4) # [1,3,2,4]
```
### 2. extend()

Add multiple elements(another list)

```bash
nums = [1,2]
nums.extend([3,4])  # [1,2,3,4]
```

### 3. insert()

Insert element at specific index

```bash
nums = [1,2,3]
nums.insert(1,4) # [1,4,2,3]
```

### 4. remove()

Remove first occurrence of value.

```bash
nums = [1,2,2,3]
nums.remove(2) # [1,2,3]
```

### 5. pop()

Remove element by index (default last)

```bash
nums = [1,2,3]
nums.pop()  # [1,2]
nums.pop(0) # [2]
```

### 6. clear()

Removes all elements

```bash
nums = [1,2,3]
nums.clear()    # []
```
OR

`del` keyword can also delete the list completely.

```bash
nums = [1,2,3,4,5]
del nums[1] # [1,3,4,5]
del nums 
print(nums) # error because you have deleted "nums" 
```

### 7. index()

Return index of first occurrence

```bash
nums = [1,2,3]
nums.index(2)   # 1
```

### 8. count()

Counts occurrence

```bash
nums = [1,2,2,3]
nums.count(2) # 2
```

### 9. sort()

Sort list(modifies original list)

```bash
nums = [3,1,2]
nums.sort()  # [1,2,3]
```

### 10. reverse()

Reverse list

```bash
nums = [1,2,3]
nums.reverse()  # [3,2,1]
```

### 11. copy()

Method `copy()` to copy a list

```bash
nums1 = [1,2,3]
nums2 = nums1.copy()
print(nums2)    # [1,2,3]
```
---
| Function   | Description              | Example              |
|------------|--------------------------|----------------------|
| `len()`    | Return number of elements| `len(nums)` # 3     |
| `max()`    | Return largest element   | `max(nums)` # 3     |
| `min()`    | Return smallest element  | `min(nums)` # 1     |
| `sum()`    | return sum of elements   | `sum(nums)` # 6     |
| `sorted()` | return new sorted list(original unchanged) | `sorted(nums)` # [1,2,3] |

## Important Notes:

- `sorted()` does not modified the original list.
- `sum()`,`max()` and `min()` work only if elements are numeric (or comparable).
- `len()` works for all sequences (list, tuple, string etc.).


---

