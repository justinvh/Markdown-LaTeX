# Markdown-LaTeX
This [Markdown](http://daringfireball.net/projects/markdown/) extension adds support for inline LaTeX expressions.

## Modes
Markdown-LaTeX can technically allow for any sort of LaTeX expression, but there are three main modes that make writing everything much easier.

### %TEXT% mode
The most basic of the modes is %TEXT% mode. Any expression within %TEXT% will be parsed in a basic LaTeX text-mode, e.g. plain. For example, %"Justin Bruce Van Horne"%.

### $MATH$ mode
Math mode is our second basic functinality of Markdown-LaTeX. It automatically puts LaTeX into math mode and allows for inline and multiline expressions. Let's say that we wanted to write [Euler's formula](http://en.wikipedia.org/wiki/Euler's_formula): We would then write $e^{\imath x} = \cos{x} + \imath\sin{x}$.

### %%PREAMBLE%% mode
Preamble mode is the only "complex" mode. It allows you to add to the preamble of the LaTeX template. So, if there are specific packages or commands you want for the HTML page, then this is where to do it. This is a global modifier and will affect the entire document. I haven't come up with an intuitive design for a per-expression basis.

## Dependencies
Markdown-LaTeX depends on:

- [LaTeX](http://www.latex-project.org/)
- [dvipng](http://sourceforge.net/projects/dvipng/)
- [Python Markdown](http://www.freewisdom.org/projects/python-markdown/)

## Installation
You can either copy it into the extensions sub-directory in your markdown folder (ex: /usr/lib/python2.7/site-packages/markdown/extensions/latex.py) or use it locally with the mdx_ prefix. See [Markdown Extensions](http://www.freewisdom.org/projects/python-markdown/Writing_Extensions) for more details.

## Usage
    markdown -x latex somefile.markdown > somefile.html

----

## How does it work?
The LaTex extension will search for either $text$ or %text% expressions. For each expression, it generates a tex file that is parsed by latex and then run through dvipng. The data is encoded via base64 and then inlined.  A cache file (latex.cache) is used to store all expressions and their base64 counterparts. This is to prevent latex from being run each time.

----

## Thanks to:
- [Geremy Condra](https://github.com/debatem1)
