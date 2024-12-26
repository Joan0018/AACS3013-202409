# How To Identify Repeating Group in 1NF for normalisation ❓
> [!IMPORTANT]
> 💥We can actually observe the repeating group from the structure of the table💥

## 1st type of Table Structure
![image](https://github.com/user-attachments/assets/f72d0df9-bf31-4120-b283-7f3d2fcf6b42)
> [!NOTE]
> When looking at rows of data from left to right, if a main row has smaller rows nested within it, we treat the starting column of those nested rows as a repeating group. This repeating group's first column acts as a second identifier (or second primary key) in 1NF.

### Example
![image](https://github.com/user-attachments/assets/3a514099-5e5c-417c-a442-8da5fc4b21d5)



## 2nd type of Table Structure
![image](https://github.com/user-attachments/assets/1fd7a057-a25f-4164-b4dc-fd80d4f9c094)
> [!NOTE]
> Reading data from left to right, within the same main identifier, any change in column data consider a repeating group. This repeating group's first column acts as a second identifier (or second primary key) in 1NF.

### Example
![image](https://github.com/user-attachments/assets/41042019-ed74-419a-be77-288f7842d3b2)
