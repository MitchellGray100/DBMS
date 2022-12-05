# DBMS

## Team 
Our team consisted of:<br>

[Mitchell Gray](https://github.com/MitchellGray100);<br>
[Jacob Kerr](https://github.com/jakejack13);<br>
[Owen Ralbovsky](https://github.com/owenxr);<br>

## Disclaimer
We sadly can't upload any source code since the project was for a class project which would lead to an academic integrity violation; however, source code can be requested by job recruiters!

## Project Description
Our team created a Data Base Management System in Java. The DBMS uses JSqlParser to parse SQL queries. Queries are transformed into Logical Query Plans and then turned into Physical Query Plans to choose the best operators for a specific query. Queries are evaluated and then outputted to corresponding result files. The datasets the DBMS worked on could be huge since we implemented, both, in-memory and external processing. Database files were read and result files were written using Java.NIO. This heavily optimized how quickly io functioned since it all operated in binary. We implemented In Memory Join, Block Nested Loop Join, and Sort Merge Join for our physical join operators. Our Interpreter implemented B+ tree indexes that could be stored/loaded via serialization/deserialization. Trees could also be made using Bulk Loading. Query plans were optimized by using statistics to change how join and select operators were place. To optimize joins, we used these statistics to create a dynamic programming algorithm that allowed us to optimize the order in which we join tables by using V-values. To optimize select operators, we used custom-made union-find data structure to push selections up the query plan tree.


