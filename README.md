# mandelwhat

A basic Clojure implementation of an ASCII Mandelbrot fractal generator.  It
would probably be really cool to print out a massive version of this and hang
it on the wall if I had some free time.

## Usage

```sh
> lein repl

user=> (use 'mandelwhat.core)

# Print canned test pattern
user=> (show-mandelbrot (mandelbrot-test))

# Use custom world rect
user=> (show-mandelbrot (mandelbrot-render {:x -1.5 :y -0.5 :w 1 :h 1}))

# Use custom world rect and custom view rect
user=> (show-mandelbrot (mandelbrot-render {:x -1.5 :y -0.5 :w 1 :h 1} {:x 0 :y 0 :w 150 :h 90))
```

## License

Copyright © 2017 David Hughes.  Distributed under the MIT license.
