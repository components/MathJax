# mathjax-component-builder

A simple script to populate the
[mathjax components repo](https://github.com/components/MathJax).
This clones [MathJax][] and the [MathJax-grunt-cleaner][] repos,
then iterates through each MathJax release tag,
making a corresponding tag on the component repo after running the `grunt component`
command, which strips out the png image fonts.
Any tags already present on the components repo are not updated.

To use:

    ./update-mathjax-component

[MathJax]: https://github.com/mathjax/MathJax
[MathJax-grunt-cleaner]: https://github.com/mathjax/MathJax-grunt-cleaner
