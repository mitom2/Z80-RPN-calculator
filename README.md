
# Z80 RPN Calculator
This project is a Reverse Polish Notation (RPN) calculator implemented in [SZAMAN](https://github.com/mitom2/SZAMAN) for custom Z80 PC. The calculator supports basic arithmetic operations like addition, subtraction, multiplication, and division, leveraging the stack to handle operands and operators in RPN format.


## Features

- Basic Integer Arithmetic: Addition, subtraction, multiplication, and division.
- Stack-based Operations: Operands and results are handled via a stack.

## Hardware Interface
This program is written with specific, custom hardware in mind. It interfaces with:
- GPU module: For display and drawing pixels, lines, rectangles and characters.
- I/O module: For managing device interactions, such as input from HID devices and storage devices.
- Memory module: For managing multiple pages of memory.

For more information see related project: [ZOE](https://github.com/mitom2/ZOE).
## Usage

Compile using [SZAMAN](https://github.com/mitom2/SZAMAN):
```bash
./SZAMAN -i system.ia -o calculator.os
```
Load the compiled file to your hardware system, or use [ZOE](https://github.com/mitom2/ZOE) for testing.
## Examples
Input:
```bash
5 3 +
```
Output:
```bash
=8
```

Input:
```bash
4 7 -
```
Output:
```bash
=-3
```

Input:
```bash
2 3 4 * + 2 /
```
Output:
```bash
=7
```

## License
This project is licensed under the terms of the MIT license. Check the LICENSE file for details.

