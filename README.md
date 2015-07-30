# mathjax-component-builder

A simple script to populate the [mathjax components repo]().
This clones [MathJax][] and the [MathJax-grunt-cleaner][] repos,
then iterates through each MathJax release tag,
making a corresponding tag on the component repo after running the `grunt component`
command, which strips out the png image fonts.

Any tags already present on the components repo are not updated.

To use:

    ./update-mathjax-component

TODO:

- Since the component repo doesn't exist yet, this pushes
  [here](https://github.com/minrk/components-mathjax)
- The `grunt component` command
  [hasn't been merged yet](https://github.com/mathjax/MathJax-grunt-cleaner/pull/5),
  so this fetches that PR instead of the master branch.

[MathJax]: https://github.com/mathjax/MathJax
[MathJax-grunt-cleaner]: https://github.com/mathjax/MathJax-grunt-cleaner
