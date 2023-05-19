# Minimum-Polymer-Tests
## Expected Output
```
All files run successfully. Beginning Tests:
Starting Run: Incorrect Atomic Number Spec
--------------------------------------------------
Invalid atom smarts found in substructure smarts for PE:
[C&D4&+0:9](-[#1&D1&+0:10])(-[#1&D1&+0:11])(-[#6&D4&+0:12](-[#1&D1&+0:13])(-[#1&D1&+0:14])-[*:15])-[*:16]
^^^^^^^^^^^
REASON: required primitive(s) not included: ['#']
--------------------------------------------------

Starting Run: Incorrect Connectivity
--------------------------------------------------
Invalid atom smarts found in substructure smarts for PE:
[#6&D3&+0:9](-[#1&D1&+0:10])(-[#1&D1&+0:11])(-[#6&D4&+0:12](-[#1&D1&+0:13])(-[#1&D1&+0:14])-[*:15])-[*:16]
^^^^^^^^^^^^
REASON: query does not match rdchem.Mol reading of the molecule (likely due to incorrect/ambiguous connectivity)
--------------------------------------------------

Starting Run: No Formal Charge
--------------------------------------------------
Invalid atom smarts found in substructure smarts for PE:
[#6&D4&+0:9](-[#1&D1&+0:10])(-[#1&D1&+0:11])(-[#6&D4:12](-[#1&D1&+0:13])(-[#1&D1&+0:14])-[*:15])-[*:16]
                                              ^^^^^^^^^^
REASON: [#6&D4:12]: no charge primitive (+ or -) on atom
--------------------------------------------------

Starting Run: Unspecified Bond Type
--------------------------------------------------
Invalid bond smarts found in subsucture smarts for PE:
SMARTS: ~       BONDTYPE: UNSPECIFIED
The only currently supported bond types are:
        SINGLE
        DOUBLE
        TRIPLE
        QUADRUPLE
        QUINTUPLE
        HEXTUPLE

--------------------------------------------------

Starting Run: Duplicate Entry Names
--------------------------------------------------
The following keys were found to be duplicate:
        LEU
Do not use standard residue names when naming custom substructures
--------------------------------------------------

Starting Run: Ambiguous Bond Info Assigned
--------------------------------------------------
Ambiguous chemical information assigned for residue PE_wrong for molecule bond (0, 4) and query bond (0, 3):
        Bond order of new query (DOUBLE) does not match the bond order of previous query (SINGLE)
--------------------------------------------------

Starting Run: Ambiguous Bond Info Assigned
--------------------------------------------------
Ambiguous chemical information assigned for residue PE_wrong for molecule atom 4 and query atom 3:
        Formal charge of new query (1) does not match the formal charge of previous query (0)
--------------------------------------------------
```
