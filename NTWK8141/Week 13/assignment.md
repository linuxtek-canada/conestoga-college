## Week 13 Slide 21

## Week 13 Slide 34
Complete the Real World Scenario: Installing the MariaDB Server on Your Ubuntu System in Ch 21

## Week 13 Slide 37
Steps 5-10

Reading/Books

* ID - Integer (ISBN)
* Title - Text
* Author - Text
* Publisher - Text
* Date - Publish Date
* Genre (Fiction, Nonfiction, History, Textbook) - Text

Database Name:  Library

# Give user permissions to database server
# As the root user (no username)

`GRANT ALL ON *.* TO 'sysadmin';`

# Create Database
`CREATE DATABASE library;`

# Use Database
`USE library;`

# Create Table

```
CREATE TABLE books (
    id int not null,
    title text,
    author text,
    publisher text,
    date date,
    genre text,
    primary key (id));
```

# Populate the Database - 3 Rows

```
INSERT into books values (1,"Neuromancer","William Gibson","Ace","1984-07-01","Cyberpunk, Fiction");
INSERT into books values (2,"Fool Moon","Jim Butcher","Penguin Putnam","2001-01-01","Fantasy");
INSERT into books values (3,"The Last Wish","Andrzej Sapkowski","Supernowa","1993-01-01","Fantasy");
```