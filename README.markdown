# Markdown-LaTeX
This [Markdown](http://daringfireball.net/projects/markdown/) extension adds support for inline LaTeX expressions.

## Modes
Markdown-LaTeX can technically allow for any sort of LaTeX expression, but there are three main modes that make writing everything much easier.

### %TEXT% mode
The most basic of the modes is %TEXT% mode. Any expression within %TEXT% will be parsed in a basic LaTeX text-mode, e.g. plain. For example, %"Justin Bruce Van Horne"% will output: <img class='latex-inline math-false' alt='klzzwxh:0000klzzwxh:0001Myklzzwxh:0002nameklzzwxh:0003isklzzwxh:0004Justinklzzwxh:0005Bruceklzzwxh:0006Vanklzzwxh:0007Horne' id='MynameisJustinB' src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARYAAAAQBAMAAAAhTU3VAAAAMFBMVEX///8AAACqqqru7u7MzMy6urqYmJjc3NwiIiKIiIhmZmYQEBAyMjJUVFR2dnZEREScQq9XAAADSklEQVRIx82VTUgUYRjH/8xns62zg1pLS+lcOnibiiA7rRRSiblCZIeopWBLydBLVqcNCtJDTR+UFpUdzCywrUMHCdkiooTMS0FCMBFlUtmaUNSl3uedGZ2VxeyU7+l9/u9/nuf3fg6wgJpgbdxy1wLCMXNOXyjtdcQvy5OFdOn64MQvq0CByXZID7tnBOntYPxzuT3LVr/hPtYiicsseW1mbmYtN91dNqPaAT2SQ1G6wJeLGUd1UAjnIERnu3bs7YCptuBqFqjIzHspAyy5gMxY5CWFVpRldv7KAlPA/m3tuBj9RxY1Lrbxxcrkswil1PFH/T0png+LGlfQanbAHoZcmVGOJQ8/ZurO441TONSUlJ9WX1vdZGN9F2WqS+NsheOx1BnaAIXNZWN1afJZLss6R3ixK8dH9b5zYt9V7j8NOaGmbriJp1n0C+/IzEVWQsNed9c7IbApVkHj87iH1xjCCdSYRVMowSP0kWoISdFnkQzcolDOUJf56CRGnqSesX1fmaVR9GM0bIb4CT1j6Qh3L0rwxMQycOtOFC+xziIziazEGrS4LKviaxnLoqTCV6uEpdrDkrVaoRGUygZ2kmooP5Dw94hVo5CxsC7zdbvrEsqyCfFRluRsPeQs+VfZlVDMkMMT++vCgIucKreaV8JliXSbjEXJNnAWmpb0YRitYDVKtfupS676cAABFgo9FvgsYhlq3ASKAVxONfKrHMnuA7YecPhXPouWZuSe2SvhsggZYhGj9jTLV6vfZ3HvqWqI0v6RAAuFckbKY8EDbJph6fRfmKgDfSpUgMUza+ngK7EsTlfijemzSCXob3NZ2GJKXNUsMI9ajKVkGaVQzij5LCs8llE1CpXtQJznL0+iygqNtQVZ2L5EHI/FK8Gbg5v8etYgwDLU4LLgJypdFoeeE7VYLgEMPKdQNYQ8Fr2UWGgUo9Aitui+rtctxhLuyWPBNxy2PBavBLXa8sRm8WMsAZ2Hu2NHTtpXGje9n+ztbD9antDHKWNtTOk6SEd9ezObbFPq03cKvzi1MZl87KLdHpz4HZcne/hoTu+zMdHlFWAv0avzp3hi+geUxT+vsPXxXjJz0S2R1xoWzF+yaMReMCzyeMv/BfgDlQMgJVk5s0IAAAAASUVORK5CYII='>. Expressions may also be multiline.

### $MATH$ mode
Math mode is our second basic functinality of Markdown-LaTeX. It automatically puts LaTeX into math mode and allows for inline and multiline expressions. Let's say that we wanted to write [Euler's formula](http://en.wikipedia.org/wiki/Euler's_formula): We would then write $e^{\imath x} = \cos{x} + \imath\sin{x}$ which outputs <img class='latex-inline math-true' alt='eklzzwxh:0097klzzwxh:0098klzzwxh:0099mathklzzwxh:0100xklzzwxh:0101klzzwxh:0102klzzwxh:0103klzzwxh:0104klzzwxh:0105osklzzwxh:0106xklzzwxh:0107klzzwxh:0108klzzwxh:0109klzzwxh:0110klzzwxh:0111mathklzzwxh:0112inklzzwxh:0113xklzzwxh:0114' id='eimathxcosximat' src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAIoAAAANBAMAAACEHOs3AAAAMFBMVEX///8AAADc3NyIiIiqqqrMzMxERERmZmYiIiJ2dnaYmJju7u4QEBC6urpUVFQyMjL8RwvRAAABdklEQVQoz6WTv0sCYRjHv9x52nneJS0NNSjOwTtEZUI0HAQOca5SIA1S1CBoVC65BIEgkRHkkmQEDsI1RktD7QZRQdBPSGyS/oKeN/K3JdW7PZ/nfT/PD+6Av57VVmB/xlXc2/Wd3BSNtKaLc0oxM9TVov2cFirAO/5rsenCXUJtaj7qQzpvirq3o4W4NI+HjdxilXh0JhfUeCzbaFlDSSsqST9OKDhczrO6xTINcB6AdI4XWupUMA0phEjt8WuYDoXCAIYDQPnIRR2K2Ne26pbZY4BzN7+1AjC5UkbPjr99RLsTGAPWewdJKfGKvMLSZwVjAuCcLE5uMTRq1N1pUVWLGUzx8KJpLxRxXrXAYYDGg1l7zQcKP9JEfRAugQUfHESlM8WsW9SEAc5rlhmcwmEqrL2ZEkTrpJD0wgrcyiGxoRcby4LzL4ua2AWDGtM7faZRhr1RV258G7gvxA4aLJYMQFx6ilz3ezaZ+nbjd/3mz7F9m/kAR19YI3yDKdYAAAAASUVORK5CYII='>.

### %%PREAMBLE%% mode
Preamble mode is the only "complex" mode. It allows you to add to the preamble of the LaTeX template. So, if there are specific packages or commands you want for the HTML page, then this is where to do it. This is a global modifier and will affect the entire document. I haven't come up with an intuitive design for a per-expression basis.

## Dependencies
Markdown-LaTeX depends on:
- LaTeX
- dvipng
- Python Markdown

## Installation
You can either copy it into the extensions sub-directory in your markdown folder (ex: /usr/lib/python2.7/site-packages/markdown/extensions/latex.py) or use it locally with the mdx_ prefix. See [Markdown Extensions](http://www.freewisdom.org/projects/python-markdown/Writing_Extensions) for more details.

## Usage
    markdown -x latex somefile.markdown > somefile.html

----

## How does it work?
The LaTex extension will search for either $text$ or %text% expressions. For each expression, it generates a tex file that is parsed by latex and then run through dvipng. The data is encoded via base64 and then inlined.


A cache file (latex.cache) is used to store all expressions and their base64 counterparts. This is to prevent latex from being run each time.

## Issues
If you screw up the LaTeX in the document, chances are you are going to get a funny output or even nothing at all. This is due to the way LaTeX handles errors. For the most part hitting "q" at a broken terminal and then consulting the resulting logfile is your best bet for sanity.

----

## Thanks to:
- [Geremy Condra](https://github.com/debatem1)
