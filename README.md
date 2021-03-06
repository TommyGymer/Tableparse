# Tableparse
---
A stand alone library which parses an array and a set of headers into a text based table

## Features

- tableparse.tablify(2D array of strings)
Takes a 2D array of strings and returns a string containing the table

e.g.
```bat
>>> array = [
>>> ["Title", "Description"],
>>> ["Macbeth", "A play by Shakespear"]
>>> ]

>>> print(tableparse.tablify(array))
╔═══════╦═════════════════════╗
║Title  ║Description          ║
╠═══════╬═════════════════════╣
║Macbeth║A play by Shakespeare║
╚═══════╩═════════════════════╝
```

---

## Installation

```bat
pip install tableparse
```

---

## Usage

```py
import tableparse

array = [
    ["Name", "Description", "URL"],
    ["TableParse", "A stand alone table generators", "https://github.com/TommyGymer/Tableparse"],
    ["JSChess", "A stand alone JS chess implementation", "https://github.com/TommyGymer/JS-Chess"],
    ["Dijkstra Pathfinding", "An implementation of Dijkstra's pathfinding algorithm", "https://github.com/TommyGymer/Dijkstra-pathfinding"]
]

result = tableparse.tablify(array)
```

### tablify

Turns a 2D array into a table string

![Tablify](https://tommygymer.github.io/Tableparse/img/tablify.jpg)

### tablify_str

```py
length = 2000
result = tableparse.tablify_str(array, length)
```

Returns a list of strings containing a table split in the 'length' characters

![Tablify_str](https://tommygymer.github.io/Tableparse/img/tablify_str.jpg)

### inv_array

```py
inv_array = tableparse.inv_array(array)

result = tableparse.tablify(inv_array)
```

Flips an array's columns and rows

![array inverse](https://tommygymer.github.io/Tableparse/img/inv_array.jpg)