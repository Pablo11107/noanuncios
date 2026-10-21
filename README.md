# PDF Cleaner

PDF Cleaner is a tool designed to remove advertisements from PDFs, making it easier to read and navigate documents without being disrupted by unwanted ads.

This tool does not just crop the ads out of the PDF, instead, we extract the original file without ads by manipulating the internal structure of the PDF, ensuring maximum quality.

In addition to removing advertisements, PDF Cleaner is also capable of extracting metadata, such as the author, subject, university, and more, from the file.

# Installation

To install PDF Cleaner, please [download](https://www.python.org/downloads/) and [install](https://wiki.python.org/moin/BeginnersGuide/Download) Python and then run the following command in your terminal:

```
pip install pdfcleaner
```

# Usage

PDF Cleaner can be used through both a Command Line Interface (CLI) and in your code.

## Command Line Interface

To use PDF Cleaner through the CLI, simply run the following command, replacing `<filename>` with the name of one or more PDF files or folders containing PDF:

```
pdfcleaner [-r] [-s] [-n] [-h] [-v] <filename>...
```

## Options

PDF Cleaner provides several options for its usage:

> - '-r': Replace the original file with the cleaned version.
> - '-s': Do not show metadata about cleaned files.
> - '-n': Force the naive cleaning method.
> - '-h': Display the help message, providing information on how to use PDF Cleaner.
> - '-v': Display the current version of PDF Cleaner.

## Code

To use PDF Cleaner in your code, you can use the following code snippet:

```python
from pdfcleaner.clean import clean_pdf_path

return_msg = clean_pdf_path("input.pdf","output.pdf")
```

## Rust Distribution

If you are willing to use the Rust distribution of PDF Cleaner, you can find the instructions in the [Rust distribution README.md](pdfcleaner_rs/README.md) file.

## WASM Distribution

If you are willing to use the WASM distribution of PDF Cleaner, you can find the instructions in the [WASM distribution README.md](pdfcleaner_wasm/README.md) file.

# License

PDF Cleaner is distributed under the GPL-3 license, which means it's open-source and free to use.

# Contributing

We're always looking for ways to improve PDF Cleaner, and we welcome contributions from the community. If you have ideas for improvements or bug fixes, please feel free to submit a pull request.

## TODO

If you want to help, these are the top priorities right now:

- Find a way to sending the method code to JS in the WASM implementation. Serialization using Serde seems to fail for some reason.
