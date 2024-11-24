# Database Design Language (DBDL)

>[!IMPORTANT]
>You need to remember **THREE (3)** way to differentiate the keys in DBDL.

<details>
<summary>Primary Key</summary>
<br>
Use underline to present it in DBDL.
  <br><br>
 Example: 
 <br>
 <ins>variable_name</ins>
</details>

<details>
<summary>Foreign Key</summary>
<br>
Use asterisk (*) to present it in DBDL.
  <br><br>
 Example: 
 <br>
 variable_name*
</details>

<details>
<summary>Composite Key</summary>
<br>
Use asterisk and underline to present it in DBDL.
  <br><br>
 Example: 
 <br>
 <ins>variable_name*</ins>
</details>

## Syntax of Database Design Language (DBDL)
<code>table_name(column_name1, column_name2, column_name3, ....)</code>

### Example
Customer(<ins>cust_id</ins>, cust_name, cust_email, cust_address, cust_phoneNumber)
<br>
Order(<ins>order_id</ins>, order_desc, order_qty, total_amount, cust_id*)

 

