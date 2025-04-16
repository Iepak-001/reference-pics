# Reference_pics

### This repo contains pics for quick revison and references to the previous studied resources for **QUICK VISUALISATION**

# HTML/CSS


![](./images/forms.png)

![](./images/Html_elements.png)

![](./images/image1.png)

![](./images/input_types.png)

![](./images/text_fields.png)

# SQL

- SQL keywords are NOT case sensitive: select is the same as SELECT

- Use semicolon at the end of each SQL statement

- How to Test for NULL Values?

It is not possible to test for NULL values with comparison operators, such as =, <, or <>.

We will have to use the IS NULL and IS NOT NULL operators instead.

- The BETWEEN operator selects values within a given range. The values can be numbers, text, or dates.

    SELECT * FROM Products  
    WHERE ProductName BETWEEN   'Carnarvon Tigers' AND    'Mozzarella di Giovanni'  
    ORDER BY ProductName;  

- NOT BETWEEN Example

    To display the products outside the range of the previous example, use NOT BETWEEN:

### ALIASES

- Note: Single or double quotation marks are required if the alias name contains spaces:

### JOIN STATEMENTS

A JOIN clause is used to combine rows from two or more tables, based on a related column between them.

![](./images/sql_joins.png)


### Update Table

UPDATE Customers  
SET ContactName = 'Alfred Schmidt', City = 'Frankfurt'  
WHERE CustomerID = 1;  

![](./images/sql_commands.png)

![](./images/sql_fiels_types.png)

![](./images/sql_insert.png)

![](./images/sql_limit.png)

![](./images/sql_nestedOrdering.png)

![](./images/sql_where.png)

![](./images/sql_wildcards.png)

- The IN operator allows you to specify multiple values in a WHERE clause.

    The IN operator is a shorthand for multiple OR conditions.

![](./images/sql_in.png)

# GRAPHS

## Dijkstra's Algo

- Finds shortest distance from source to all other nodes

- Doesn't work with **Negative Weights** 

- TC: O(V + E log V) with min-heap

### Approaches

#### Naive

![](./images//graph_dij_basic.png)

#### Use Queue with in_queue Marking

![](./images/graph_dij_queue.png)

#### Use PQ

![](./images/graph_dij_pq.png)

#### Using SET

![](./images/graph_dij_set.png)

## Bellman Ford

- Improvement from Dijkstra to handle *Negative Weights*

- Can also detect *Negative Cycles*

- TC: O(V × E)

- Algorithm

    - Let n = no of nodes

    - Saare edges pr (n-1) times distance check kro

    - To detect negative cycle

        - saare Edges pr one time more dist check kro

        - If any distance gets updated => Negative cycle present

 ![](./images/graph_bellman.png)


## Floyd-Warshall

- All pair Shortest-Path

- Handles Negative weights

    - *** If No Negative Wt Present *** Then apply Dijkstra on each node

- Detect Negative Cycles

- TC: O(V³) where V=No of vertices(Nodes)

- Algorithm

![](./images/graph_floyd_Idea.png)

 ![](./images/graph_floyd.png)