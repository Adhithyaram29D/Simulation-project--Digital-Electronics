# TITTLE
Minimise the function using K map F(A,B,C)=A′B+BAC′+A'B′C′ and simulate the logic diagram using verilog
# THEORY
### THE KMAP
The K-map method is particularly useful for reducing complex logic functions, especially those with multiple variables, into a simplified form. By grouping adjacent cells that have the value of 1, known as minterms, patterns and common terms can be identified. These groupings can then be used to derive a simplified Boolean expression that requires fewer logic gates to implement.

The Karnaugh map follows specific rules for grouping cells: the groups must be rectangular in shape and their sizes must be powers of 2 (1, 2, 4, 8, etc.). Each group should encompass as many minterms as possible, while still being adjacent in the grid. By combining these groups, redundant terms can be eliminated, resulting in a minimized expression.

Using the K-map method helps to reduce the complexity and size of logic circuits, which in turn can lead to improved performance, reduced power consumption, and easier circuit design. It is a visual and intuitive technique that simplifies the process of logic minimization, allowing designers to optimize digital systems efficiently. The Karnaugh map is widely used in fields such as computer engineering, digital electronics, and computer science to achieve optimal logic circuit design.

# LOGIC DIAGRAM
![Screenshot 2023-06-14 132443](https://github.com/Adhithyaram29D/Simulation-project--Digital-Electronics/assets/119393540/743f7ed5-25e7-4d43-86fe-2e62179ca593)

# NETLIST DIAGRAM
![Screenshot 2023-06-14 132443](https://github.com/Adhithyaram29D/Simulation-project--Digital-Electronics/assets/119393540/743f7ed5-25e7-4d43-86fe-2e62179ca593)

# TIMING DIAGRAM
![Screenshot 2023-06-14 133020](https://github.com/Adhithyaram29D/Simulation-project--Digital-Electronics/assets/119393540/64b7a95a-fc16-48a4-91fd-92c93ab463dc)

# PROGRAM
```
module skill2(a,b,c,F);
input a,b,c;
output F;
wire adash,cdash,x,y,z;
not(adash,a);
not(cdash,c);
and(x,adash,b);
and(y,b,cdash);
and(z,adash,cdash);
or(F,x,y,z);
endmodule
```
# SIMPLIFICATION
![tinywow_Document 98_26539481_1](https://github.com/Adhithyaram29D/Simulation-project--Digital-Electronics/assets/119393540/47d835a1-c329-4ffd-90c1-1c353de9350d)

