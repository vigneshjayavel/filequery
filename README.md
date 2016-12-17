# filequery
SQL interface for finding files. Linux "find" command on steroids.

**What if we can do the following on the linux command line?**

```SQL
select count(*) from '~/music' where created_at > '2016-12-12'

select file_type, count(*) as cnt from '~/downloads' group by file_type

select count(*) from '/' where file_content like "%my sample content%"

select sum(file_size) from '/' where file_type in ('txt','md')
```

Inspiration behind this project is [gitql](https://github.com/gitql/gitql)



