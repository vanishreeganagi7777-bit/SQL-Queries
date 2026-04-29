# SQL-Queries
Create table table name(id datatype(length), ………);
use tech;
select * from employee;

insert into employee values
(101, 'Jan', 'Levison', '1961-05-11', 'F', 110000, null, null);<br>
insert into employee values
(102, 'Michael', 'Scott', '1964-03-15', 'M',75000, null, null);<br>
insert into employee values
(103, 'Angela', 'Martin', '1971-06-25', 'F', 63000, null, null);<br>
insert into employee values
(104, 'Kelly', 'Kapoor', '1980-02-05', 'F', 55000, null, null);<br>
insert into employee values
(105, 'Stanley', 'Hudson', '1958-02-19', 'M', 69000, null, null);<br>
insert into employee values
(106, 'Josh', 'Porter', '1969-09-05', 'M', 78000, null, null);<br>
insert into employee values
(107, 'Andy', 'Bernard', '1973-07-22', 'M', 65000, null, null);<br>
insert into employee values
(108, 'Jim', 'Halpert', '1978-10-01', 'M', 71000, null, null);<br>

select * from employee;

insert into branch values(2, 'Scranton', 100, '2006-02-09');<br>
insert into branch values(3, 'Stamford', 106, '1998-02-13');<br>

UPDATE branch
SET mgr_id = 102,
    mgr_start_date = '1992-04-06'
WHERE branch_id = 2;

Update employee set super_id=100, branch_id=1 where emp_id=101;
Update employee set super_id=100, branch_id=2 where emp_id=102;
Update employee set super_id=102, branch_id=2 where emp_id=103;
Update employee set super_id=102, branch_id=2 where emp_id=104;
Update employee set super_id=102, branch_id=2 where emp_id=105;
Update employee set super_id=100, branch_id=3 where emp_id=106;
Update employee set super_id=106, branch_id=3 where emp_id=107;
Update employee set super_id=106, branch_id=3 where emp_id=108;

select * from employee;


insert into client values(400, 'Dunmore HighSchool', 2);<br>
insert into client values(401, 'Lackawana Country', 2);<br>
insert into client values(402, 'FedEx', 3);<br>
insert into client values(403, 'John Daly Law, LLC', 3);<br>
insert into client values(404, 'Scranton Whitepages', 2);<br>
insert into client values(405, 'Times Newspaper', 3);<br>
insert into client values(406, 'FedEx', 2);<br>

select * from branch_supplier;

insert into branch_supplier values(2, 'Hammer Mill', 'Paper');<br>
insert into branch_supplier values(2, 'Uni-ball', 'Writing Utensils');<br>
insert into branch_supplier values(3, 'Patriot Paper', 'Paper');<br>
insert into branch_supplier values(2, 'J.T.Forms & Labels', 'Custom Forms');<br>
insert into branch_supplier values(3, 'Uni-ball', 'Writing Utensils');<br>
insert into branch_supplier values(3, 'Hammer Mill', 'Paper');<br>
insert into branch_supplier values(3, 'Stamford Labels', 'Custom Forms');<br>

select * from branch_supplier;

insert into works_on values(105,400,55000);<br>
insert into works_on values(102,401,267000);<br>
insert into works_on values(108,402,22500);<br>
insert into works_on values(107,403,5000);<br>
insert into works_on values(108,403,12000);<br>
insert into works_on values(105,404,33000);<br>
insert into works_on values(107,405,26000);<br>
insert into works_on values(102,406,15000);<br>
insert into works_on values(105,406,130000);<br>

select * from works_on
