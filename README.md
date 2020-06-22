# python-db
Basic Python Db stuff

## Install things:
pip install -r requirements.txt

### Assumptions
* Use Pipenv & virtualenvs
* Python 3.8.2

## DB Setup
MySQL Console:
```
Create database demo;
Use demo;
create user 'testuser'@'localhost' IDENTIFIED BY 'Test123!';
```

Make some tables:
```
create table student(fname varchar(20), lname varchar(20), age int, enrolment_no varchar(12));
```

Make another table:
```
CREATE TABLE `users` (
    `id` int(11) NOT NULL AUTO_INCREMENT,
    `email` varchar(255) COLLATE utf8_bin NOT NULL,
    `password` varchar(255) COLLATE utf8_bin NOT NULL,
    PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8 COLLATE=utf8_bin
AUTO_INCREMENT=1 ;
```


Output looks like:

#### db-test.py
```
[Running] python -u "/Users/rbren264/Sites/Python/db-sql/dbtest.py"
{'id': 1, 'password': 'very-secret'}
```

#### dbtest.py
```
[Running] python -u "/Users/rbren264/Sites/Python/db-sql/db-test.py"
Database version : 8.0.19 
```