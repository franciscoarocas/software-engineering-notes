Most important information to index is how application select the data.

Based in most important index: B-tree.

## Chapter 1: Anatonomy of a index

To create index use commando: *create index*. Similar as index of a book. A index use is own space and contains a copy of the table.

An index needs to update frecuently. Its combine two structures:

* Double link list

* Search Tree

### Leaf nodes of an index

Its not possible to order the data of the table, because each insert must move big chunks of the data down. Thats why fisically its not ordered. However, the index data is ordered, this is because the double link list.

When you insert, index just move for each linkedin list, and then insert the data into the found node. Each lead node is stored in a page disk. Each node is internally ordered, also all nodes are ordered.

Nodes have records. Each record contains the value indexed and the ROWID. this rowid contains a pointer to the table row which contains all the row data.
