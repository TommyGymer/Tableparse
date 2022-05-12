# Tableparse
---
Parses an array and a set of headers into a text based table

## Features

- tableparse.tablify(2D array of strings)
Takes a 2D array of strings and returns a string containing the table

e.g.
```
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