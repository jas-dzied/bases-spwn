# bases-spwn
A library to convert numbers between any base. 

It includes a single type, `@base_number`, which you can use to hold your numbers in different bases.

# Usage

```
base_number = import bases
let binary_number = base_number::with_base(2, 6376374)
$.print(binary_number)
let back_to_number = binary_number as @number
$.print(back_to_number)
```

Most numerical operations work on the numbers as well, and they support both base_numbers and the std number:
```
binary_number += 10
$.print(binary_number)
binary_number += base_number::with_base(5, 321)
$.print(binary_number)
```

As well as comparisons:
```
test_number = base_number::with_base(10, 123)
$.print(test_number == 123)
```

# All bases up to 16 are currently supported, but more can be added if the corresponding characters are also added. (see the first 2 lines of bases.spwn)
