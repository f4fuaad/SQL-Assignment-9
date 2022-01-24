# SQL-Assignment-9

Q-1. Write an SQL query to show the top n (say 10) records of a table.

Ans  Select top 10 *
        From  Worker_table

Q-2. Write an SQL query to determine the nth (say n=5) highest salary from a table.

Ans select top 1 *
        From (select top 5 salary from worker_table 
        order by salary desc) result
        order by salary asc
