## The DVDRental Postgres Sample DB

First, download the file and put it somewhere on your drive. It's a TAR file (an archive) and you'll use it directly when loading. Remember where it is (maybe drop it in `C:\temp` if you're on windows).

To load this up, do this:

```
createdb dvdrental
```

This will create the sample DB. Then, you'll need to run pg_restore. If you're on windows this is in `C:\>cd C:\Program Files\PostgreSQL\9.3\bin` (make sure your version is correct).

If the bin is in your path, you should be able to run `pg_restor` straight away.

Now, run it:

```
pg_restore -d dvdrental C:\temp\dvdrental.tar
```

That's it - you should be good to go.
