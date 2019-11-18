This is a shell script profiler.

`shellprof` will run your program, and when the program finishes `shellprof`
will create a top list of which lines were show the longest.

# Usage
```sh
shellprof my-program --whatever --flags --myprogram --wants
```

# Development
Run `tox && ./shellprof ./testcase.sh` to lint and test the code.

For ease of distribution, `shellprof` only depends on the standard library.
