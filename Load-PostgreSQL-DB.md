### step-by-step Creating a new DVD rental database

- run below command in `psql` command line for your `demo` container. 
`CREATE DATABASE dvdrental;`

- verify the database by issuing `\l` 
![](https://github.com/manas86/postgres-tutorial/blob/master/list-dbs.png)

- Now checkin-to DB dvdrental by issuing `\c dvdrental` in your `sql` command line of `demo` container.

- Now in another window, run `docker exec -it demo bash` command to get inside the `demo`container. 

- Now download and unzip the file [dvdrental.zip](https://github.com/manas86/postgres-tutorial/blob/master/dvdrental.zip) file on your local machine. 

### DVD Rental DB:

The DVD rental database has many objects including:

* 15 tables
* 1 trigger
* 7 views
* 8 functions
* 1 domain
* 13 sequences

DVD Rental ER Model: 

![](https://github.com/manas86/postgres-tutorial/blob/master/dvd-rental-sample-database-diagram.png)

15 tables in the DVD Rental databases and their corresponding dat file:
 
| Table Name | Description | Input file name |
| --- | --- | --- |
| actor | stores actors data including first name and last name | 2163.dat |
| film | stores films data such as title, release year, length, rating, etc. | 2167.dat |
| film\_actor | stores the relationships between films and actors | 2168.dat |
| category | stores film&#39;s categories data | 2165.dat |
| film\_category | stores the relationships between films and categories | 2169.dat |
| store | contains the store data including manager staff and address | 2189.dat |
| inventory | stores inventory data | 2179.dat |
| rental | stores rental data | 2185.dat |
| payment | stores customer&#39;s payments | 2183.dat |
| staff | stores staff data | 2187.dat |
| customer | stores customers data | 2177.dat |
| address | stores address data for staff and customers | 2171.dat |
| city | stores the city names | 2173.dat |
| country | stores the country names | 2175.dat |
| language | stores the languages of film | 2181.dat |
