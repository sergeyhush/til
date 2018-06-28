# Check who is listening on a port

We can use lsof to check who is listening on a specific port

```bash
$ lsof -i TCP:5000
```

In case you just need the process PID(s) (maybe to kill it), add the 'terse' flag

```bash
kill $(lsof -ti TCP:5000)
```
