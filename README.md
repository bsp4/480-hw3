480-hw3
=======

When reworking my gcd algorithm here are the timeit values from old(gcd1) vs cython adaptation(gcd2):

timeit ("gcd1(1234321, 6787)") -- 625 loops, best of 3: 72.5 µs per loop
timeit ("gcd2(1234321, 6787)") -- 625 loops, best of 3: 8.47 µs per loop

timeit ("gcd1(1234321, 987654)") -- 625 loops, best of 3: 97.8 µs per loop
timeit ("gcd2(1234321, 987654)") -- 625 loops, best of 3: 11.4 µs per loop

timeit ("gcd1(43652321, 987654)") -- 625 loops, best of 3: 40.7 µs per loop
timeit ("gcd2(43652321, 987654)") -- 625 loops, best of 3: 4.9 µs per loop

The updated code runs about 8times faster.
