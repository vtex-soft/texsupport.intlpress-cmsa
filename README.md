# International Press book series CMSA author support

## Table of Contents

* [About](#about)
* [Package content](#package-content)
* [Setup](#setup)
* [Recomended usage of `ipbook` package](#recomended-usage-of-ipbook-package)
* [Submission](#submission)
* [Bug reports](#bug-reports)

## About

Author support service provides LaTeX style files and `*.tex` file templates designed for International Press book series
[Harvard CMSA Series in Mathematics (CMSA)](https://www.intlpress.com/site/pub/pages/books/_home/series/00000027/) manuscripts.

## Package content

The following files are given in the repository (or directly in `*.zip` archive):

* `ipbook.cls` - LaTeX style files designed for International Press book series.
  Please do not change them. These files are already loaded in the respective template files;
* `cmsa-template.tex` - topmatter template (should be used for manuscript preparation);
* `cmsa-sample.tex` - book series sample article;
* `cmsa-sample.pdf` - book series sample article (`PDF` file);

## Setup
* Clone the repository or download the `*.zip` archive. Rename the package to `<your-project-name>`.
* Install `ipbook.cls` file in your TeX system (suggested directory: `ipbook`).
* Use the file `cmsa-template.tex` to start your article as a template.
* Use the file `cmsa-sample.tex` as a reference for how to prepare a topmatter of your article.

## Recommended usage of `ipbook` package

Use `cmsa-template.tex` as a template.

### Document class options

For the CMSA journal `cmsa` option must be set
in a `\documentclass[]{ipbook}`:
```latex
\documentclass[cmsa]{ipbook}
```

### LaTeX document preamble content

The preamble of your LaTeX document should look like this:

```latex
\documentclass[cmsa]{ipbook}

\title[A sample document]{A sample document for IP book series}

\author{First Author}
\address{Address of the First Author, Country}
\email{first@somewhere.com}
\thanks{First Author is supported by ...}
\author{Second Author}
\address{Address of the Second Author, Country}
\email{second@somewhere.com}

\begin{document}

    \begin{abstract}
    ...
    \end{abstract}

    \maketitle

    \tableofcontents

    Your manuscript content

\end{document}
```

## Submission

Submit one single file as a `ZIP` archive.
Pack your root folder `<your-project-name>` with files and subfolders.

## Bug reports

Please submit bug report or feature requests at
[github](https://github.com/vtex-soft/texsupport.intlpress-cmsa/issues) page.