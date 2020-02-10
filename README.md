# Getting Started
See the Example notebook.
### Import
```
from sym_format import SymbolFormat
```
### Instantiate SymbolFormat object
```
sf = SymbolFormat()
```
### Get Object Type's identifier
```
str(sf.R)
```
'|R'

### Get ObjectType's format
```
sf.A()
```
{'A': 0,
 'x': 1,
 'y': 2,
 'size': 3,
 'rotation': 4,
 'justification': 5,
 'visible': 6,
 'value': 7}
### Get the index of an ObjectType's Field
```
int(sf.A.rotation)
```
4
### Get Field's format
```
sf.A.rotation()
```
{'Rotate0': 0,
 'Rotate90': 1,
 'Rotate180': 2,
 'Rotate270': 3,
 'MirrorH': 4,
 'MirrorH90': 5,
 'MirrorH180': 6,
 'MirrorH270': 7}

# References
Most of the formatting was found through reverse engineering the symbol files, but I did stumble on reference documentation later that I used in addition to my original effort. These documents are included in the References directory and include Viewdraw_ASCII_Database_Structure.txt edited by Juha Manninen and Martin Vana (Juha's email given in the text file no longer seems to be valid). I'm not sure who created the viewdraw_file_format.pdf document.