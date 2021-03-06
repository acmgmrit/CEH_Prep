# <center>SQL Injection(SQLi)

## What is SQL Injection...?
> * SQL injection is a web security vulnerability that allows an attacker to interfere with the queries that an application makes to its database
> * In this technique, the attacker injects malicious SQL queries into the user input form 

## What SQLi attack can do...
> * <b>Gain unauthorized access to a database</b>
> * <b>Authentication bypass</b>
>> An attacker can logs onto an application without providing valid username and password, and gains administrative priviliges
> * <b>Information Disclosure</b>
>> An attacker can disclose the sensitive information stored in the database
> * <b>Compromised Data integrity</b>
>> An Attacker can insert malicious content or alter the contents of a respective webpage
> * <b>Compromised availability of Data</b>
>> An attacker can delete the contents of the database
> * <b>Remote Code Execution</b>
>> An attacker can upload shells that can compromise the host OS
 
## Reasons for SQL Injection vulnerability
> Improper validation of user input before passing it to an SQL statement and server

## Types of SQL Injection Attacks
> * <b>In-band SQL Injection</b>
>> Attacker uses the same communication channel to perform the attack
> * <b>Blind/Inferential SQL Injection</b> 
>> * Attacker has no error messages from the system to work on
> * <b>Out-of-band SQL Injection</b>
>> * Attacker uses different communication channels such as file writing, database email functionality etc.,
![Types of SQL Injection](../assets/types_of_sql_injection.png)