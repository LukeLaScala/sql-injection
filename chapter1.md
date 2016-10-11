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

Let's take this query for example:

> ```
> select username, secret, number from users;
> ```

Let's break this down:

The `select` command grabs all the rows from the table users 

