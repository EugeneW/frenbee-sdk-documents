In principle, DateTime represents the UTC date and time for [[Frenbee Document]].

In C# code, it is a [`System.Guid`](http://docs.go-mono.com/?link=T%3aSystem.Guid) structure.
In XML representation, an integer (Int64) that increments by 1 in steps of 100 nanoseconds is used, with 0001/01/01 00:00:00 (UTC) being 0.

* Same as [`DateTime.Ticks`](http://docs.go-mono.com/?link=P%3aSystem.DateTime.Ticks)
* 100-nanosecond intervals since 0001/01/01 00:00:00 UTC
