# 📦 Product Inventory System (C)

A simple, menu-driven inventory manager written in C. It stores up to 5 products in memory using parallel arrays and lets you add, search, view, and update stock from the terminal.

## Features

- **Add Product**: store ID, name (spaces allowed), price, and quantity
- **Search Product**: look up a product by ID
- **Display All Products**: formatted table of everything in stock
- **Update Quantity**: change the stock of an existing product
- **Input handling**: inventory-full and empty-inventory checks, invalid menu choice message

## Concepts Practiced

Arrays and parallel arrays · `do-while` loop · `switch-case` · `scanf` with scan sets (`%19[^\n]`) · formatted output with `printf` · `#define` constants

## Getting Started

**Requirements:** a C compiler such as GCC (MinGW on Windows).

```bash
git clone https://github.com/YOSHITH-0312/Product-Inventory-System-C.git
cd Product-Inventory-System-C
gcc project.c -o project
```

Run it:

```bash
# Windows (PowerShell)
.\project.exe

# Linux / macOS
./project
```

## Sample Output

```
==============================
   PRODUCT INVENTORY SYSTEM
==============================
1. Add Product
2. Search Product
3. Display All Products
4. Update Quantity
5. Exit
==============================
Enter your choice (1-5): 3

ID      Name                     Price       Quantity
-----------------------------------------------------
101     Blue Pen                 10.50       50
102     Notebook                 45.00       30
```

## Known Limitations

- Holds a maximum of 5 products (change `MAX` to increase)
- Data is lost when the program exits (no file storage yet)
- No duplicate-ID or negative-value validation
- Entering letters where a number is expected can cause an infinite loop

## Future Improvements

- [ ] Save and load data from a file
- [ ] Prevent duplicate IDs
- [ ] Validate price and quantity
- [ ] Delete product option
- [ ] Use `struct` instead of parallel arrays

## Author

Made by **Yoshith**, B.Tech (AI/ML), Sreenidhi University.

## License

This project is licensed under the MIT License.
