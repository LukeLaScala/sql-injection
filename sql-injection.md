# How does SQL injection work?

### Well, let's say we have this table called users :

| **username** | **password** |
| --- | --- |
| Luke | 9wnlf8spnzkfsdufsud3rj |
| Alec | ThisIsSoSecure |
| Hiroki | SecurityAtItsFinest |
| Jamie | GetRekt |
| Sam | WowBoyNoiceJob |

So let's say there is a query that looks like this:

> `select username, password from users where username = 
> '$username' and password = '$password'`

`$username` is a variable that contains a username supplied by the user.

`$password` is a variable that contains a password supplied by the user.

### This is when it gets very interesting.

# What if the user supplied the following credentials:

`$username` = ' hello

`$password` = IThinkThisIsMyPassword

The query would now look like:

> `select username, password from users where username = '' hello' and password = 'IThinkThisIsMyPassword'`

What? How do we select a row where the username equals an empty string followed by random letters that aren't even in quotes?

And bam! SQL Injection is born.

We can now make the query do almost anything we want.

These operators will be very helpful:

`OR` and `#`

`#` comments the rest of the line out.

\#\#\#More coming soon!

