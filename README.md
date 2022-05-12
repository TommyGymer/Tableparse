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

>>> print(tableparse.tablify)
╔═══════╦═════════════════════╗
║Title  ║Description          ║
╠═══════╬═════════════════════╣
║Macbeth║A play by Shakespeare║
╚═══════╩═════════════════════╝
```

## Usage

```py
import tableparse

array = [
    ["Title", "Description", "Date"],
    ["", "", ""]
]
```