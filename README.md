*This project has been created as part of the 42 curriculum by ebansse.*

# C++ Module 07: C++ Templates

Exercises on **function templates** and **class templates** in C++98.

| Exercise | Program | Topic |
|---|---|---|
| `ex00` | `Template` | Function templates `swap`, `min` and `max` that work with any comparable type |
| `ex01` | `Iter` | `iter(array, length, func)`: applies a function to every element of an array (the element type and the function are both template parameters) |
| `ex02` | `Array` | `Array<T>`: a class template for a fixed-size array allocated with `new[]`, with deep copy, `size()`, and `operator[]` that throws `std::exception` on an out-of-bounds index |

## Build & run

```bash
cd ex02 && make
./Array
```

All exercises compile with `c++ -Wall -Wextra -Werror -std=c++98`.

## Concepts covered

- Template syntax, type deduction and instantiation
- Writing generic code in headers (`.hpp`) so the compiler can instantiate it
- Class templates with dynamic memory: deep copy, assignment operator and destructor
- Const-correct overloads of `operator[]`
