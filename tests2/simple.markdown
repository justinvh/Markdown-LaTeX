This examples illustrates using delimiters \$$, \%%, and %\%%
--------

This is math: $$\int_0^\infty e^{-x} \; d x = 1$$ <p/>
This is text: %%\LaTeX rocks, even in markdown with the latex plugin.%% <p/>

%%%
\usepackage[usenames]{xcolor}
\color{red}
%%%

This is not latex text: \%% foo \%% <p/>
This is not latex math: \$$ i^2 = -1 \$$ <p/>
This is a backslash with delimiters: \\\%%, \\%\%%, \\$$ <br/>
And again: \\\%%, \\%\%%, \\$$

