# reference-pics

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