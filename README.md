This is a shell script profiler.

`shellprof` will run your program, and when the program finishes `shellprof`
will create a top list of which lines were shown the longest.

```sh
~/s/shellprof (master|✔) $ ./shellprof ./testcase.sh
quick
slow
quick

Timings for printed lines:
1.01s: slow
0.00s: <<<PROGRAM START>>>
0.00s: quick
0.00s: quick
~/s/shellprof (master|✔) $
```

# Usage
```sh
shellprof my-program --whatever --flags --myprogram --wants
```

# Development
Run `tox && ./shellprof ./testcase.sh` to lint and test the code.

For ease of distribution, `shellprof` only depends on the Python standard library.
