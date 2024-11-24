# Keys in database design 🔑
<details>
<summary>Primary Key</summary>
<br>
1. Unique identifier for the table.
  <br><br>
2. Data cannot be duplicate.
</details>

<details>
<summary>Foreign Key</summary>
<br>
1. Referential key from another table.
  <br><br>
2. Data can be duplicate.
</details>

<details>
<summary>Composite Key</summary>
<br>
1. Combination of primary key and foreign key.
  <br><br>
2. Either one column of the data can be repeat. However, same combination cannot be duplicate.
</details>

# How to Identify Foreign Key❓

>[!IMPORTANT]
>Always remember **FOREIGN KEY** place at **MANY SITE**

# Why Foreign Key must be located at many site❓

### Example ❌
<img width="522" alt="image" src="https://github.com/user-attachments/assets/1a7c2920-bfa7-4746-b51d-784ec5ab08ad">

### Scenario 
You are the customer 'CUS001' for company A and you willing to buy a product from the company. The orders data will be recorded in the database as shown

<img width="590" alt="image" src="https://github.com/user-attachments/assets/1e7b617d-947c-44f6-8117-824b5b063e3f">

On the next day, you decide to buy another product from the same company. The orders data will be recorded in the database as shown

<img width="590" alt="image" src="https://github.com/user-attachments/assets/04c0ce19-8b01-405d-8846-ee819055c5a6">

You may found that you against the rule for the primary key where all the value of primary key in a table should be **UNIQUE** and **CANNOT DUPLICATE** ‼️

Therefore, it you placed your foreign key at **ONE** site, each of your customers will be only allow to make an order for their whole life.

## Correct Example ✅
As foreign key's data can be duplicate, therefore if you willing to show the customer is allowed to buy more than one products, always remember put your foreign key at **MANY** site.
<img width="525" alt="image" src="https://github.com/user-attachments/assets/d14fcafb-1a10-4c63-938a-4c04ee2db7f1">

### Sample Data 
<img width="590" alt="image" src="https://github.com/user-attachments/assets/0cc3c1c2-6d76-4a7f-b461-d245d68bc98a">














