# MathJax Component

This is the MathJax components repo. It contains releases of mathjax,
with the png image fonts removed, since they are often unused,
and take up a large portion of MathJax install size and time.

The master branch of this repo contains a simple script to update the
[mathjax components repo](https://github.com/components/MathJax).
This clones [MathJax][] and the [MathJax-grunt-cleaner][] repos,
then iterates through each MathJax release tag,
making a corresponding tag on the component repo after running the `grunt component`
command, which strips out the png image fonts.
Any tags already present on the components repo are not updated.

To update the tags on the components repo when a new MathJax release has been made, run:

    ./update-mathjax-component

[MathJax]: https://github.com/mathjax/MathJax
[MathJax-grunt-cleaner]: https://github.com/mathjax/MathJax-grunt-cleaner
