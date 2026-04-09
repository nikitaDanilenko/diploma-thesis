# What's that?

My diploma thesis in functional analysis.
Aside from styling and typos, the contents are the same as in the version that I have submitted in 2010.

# Why is that here?

I was reminded of the [Johnson-Lindenstrauss Lemma](https://en.wikipedia.org/wiki/Johnson%E2%80%93Lindenstrauss_lemma) 
by a recent trick that was employed in improving LLM model sizes.
A [slightly differently phrased variant](./Kapitel4/JohnsonLindenstraussLemma.tex) of the lemma is proved in the thesis.
It was unnecessarily tricky to compile everything, so I decided to improve that with the help of Copilot,
and to make it available for anytime later.

# Is it worth it?

Probably not.
The pacing is terrible, there is no proper motivation for anything,
and all tangents are extremely technical - they already assume deep familiarity with the topic!
The notation is precise, but terse.

However, there are also some interesting things inside:

1. There is a non-trivial computation of a constant, which is usually just assumed to "fit" in the literature.
2. A faulty proof from a reference book is fixed.
3. The technical stuff guards against hand-wavy arguments, and tightens various statements that are present in the original source.

# How to compile?

The usual `pdflatex` + `biblatex` + `pdflatex` + `pdflatex` should do the trick.
Alternatively, you can use `lualatex --bibtex "Diplom.tex"`.
The packages are mostly standard, so they should be available in any TeX distribution.

# How is the LaTeX?

Terrible.
While there is definitely some abstraction,
this was written in a time, where I wanted everything in one place,
and was very familiar with LaTeX.
As such, there were a lot of unnecessary commands, and the structure itself was non-standard
in a bad way.

Since there are a lot of abbreviations, and shorthands, 
an IDE may fail to resolve the mostly standard commands that are encoded.
Additionally, there is probably still a lot of shorthands, where for instance not only braces are omitted, but also the spaces between the arguments.
For example, there were examples like `f(x)^ldt` around, where `^l` is a superscript, but `dt` is the standard integration notation.
