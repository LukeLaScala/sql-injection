# What is SQL?

SQL stands for **s**tructured **q**uery **l**anguage. SQL is used to communicate with a database using query, or statements written in SQL.

### Here is a sample table titled _users_:

| **username** | **secret** | **number** |
| --- | --- | --- |
| Luke | I love jowls | 87 |
| Alec | Scarlet sucks | 64 |
| Hiroki | Like to play lol for n00bs | 5 |
| Jamie | Join the LR revolution | 76 |
| Sam | Stinks at web dev | 54 |

### Let's take this query for example:

> ```
> select username, secret, number from users where username = 'Alec';
> ```

### Let's break this down:

The `select` command grabs all the rows from the table. The `where` command limits the rows returned by the query to only those where the username is equal to 'Alec'. Therefore it would select this row only:

| username | secret | number |
| --- | --- | --- |
| Alec | Scarlet sucks | 64 |

### Let's move on to a more difficult query: 

> ```
> select * from users where username = 'Alec' or username = 'Sam';
> ```

### What does this query do?
The `*` selector grabs all columns. In this case it grabs username, secret and number. This query is much like the last one except that is will grab rows where username is 'Alec' or 'Sam'. 



