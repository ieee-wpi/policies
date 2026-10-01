# WPI IEEE Student Branch Policies

This repository contains the governing documents and operational policies of
the IEEE Student Branch at Worcester Polytechnic Institute (WPI). The
documents are maintained in LaTeX so that changes can be reviewed in plain
text and published as consistent PDF files.

## Documents

| Document | LaTeX source | PDF |
| --- | --- | --- |
| Branch Constitution | [`constitution/WPI_IEEE_Student_Branch_Constitution.tex`](constitution/WPI_IEEE_Student_Branch_Constitution.tex) | [`constitution/WPI_IEEE_Student_Branch_Constitution.pdf`](constitution/WPI_IEEE_Student_Branch_Constitution.pdf) |
| Branch Bylaws | [`bylaws/WPI_IEEE_Student_Branch_Bylaws.tex`](bylaws/WPI_IEEE_Student_Branch_Bylaws.tex) | Generated as `bylaws/WPI_IEEE_Student_Branch_Bylaws.pdf` |
| Lounge Policy | [`lounge_policy/WPI_IEEE_Student_Branch_Lounge_Policy.tex`](lounge_policy/WPI_IEEE_Student_Branch_Lounge_Policy.tex) | [`lounge_policy/WPI_IEEE_Student_Branch_Lounge_Policy.pdf`](lounge_policy/WPI_IEEE_Student_Branch_Lounge_Policy.pdf) |

## Building the PDFs

### Prerequisites

Install a LaTeX distribution that includes `latexmk` and the packages used by
the documents.

- [TeX Live](https://tug.org/texlive/) for Linux and other Unix-like systems
- [MacTeX](https://tug.org/mactex/) for macOS
- [MiKTeX](https://miktex.org/) for Windows

### Build a document

From the repository root, run:

```bash
latexmk -pdf -cd constitution/WPI_IEEE_Student_Branch_Constitution.tex
latexmk -pdf -cd bylaws/WPI_IEEE_Student_Branch_Bylaws.tex
latexmk -pdf -cd lounge_policy/WPI_IEEE_Student_Branch_Lounge_Policy.tex
```

Each PDF is written next to its corresponding `.tex` source file. To remove
LaTeX-generated intermediate files while keeping the PDFs, replace `-pdf`
with `-c` in the commands above.