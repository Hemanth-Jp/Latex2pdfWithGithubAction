LaTeX Example Project
=====================

This repository provides an example LaTeX project that demonstrates the use of sections, images, tables, mathematical equations, and a bibliography. The project is automatically compiled into a PDF using GitHub Actions, making it easy to generate the final document directly from the repository.

Features
--------

This LaTeX example includes:

- **Sections**: Structured and well-organized content.
- **Images**: Demonstrates how to include images in a document.
- **Tables**: Creates neat and organized tables with captions.
- **Mathematics**: Includes mathematical equations and formulas.
- **Bibliography**: Uses a ``.bib`` file for references with ``biblatex``.

Repository Structure
--------------------

The repository contains the following files:

+-----------------------+--------------------------------------------------------------+
| File                  | Description                                                  |
+=======================+==============================================================+
| ``example.tex``       | The main LaTeX source file for the document.                 |
+-----------------------+--------------------------------------------------------------+
| ``references.bib``    | Bibliography file containing references for citations.       |
+-----------------------+--------------------------------------------------------------+
| ``example-image.png`` | Example image used in the document (replaceable).            |
+-----------------------+--------------------------------------------------------------+
| ``.github/workflows/``| Directory containing the GitHub Actions workflow.            |
+-----------------------+--------------------------------------------------------------+
| ``README.rst``        | This file, providing an overview of the project.             |
+-----------------------+--------------------------------------------------------------+

How It Works
------------

This project uses GitHub Actions to automatically compile the LaTeX document into a PDF file whenever changes are pushed to the repository. The resulting PDF is saved as an artifact or published in the repository's Actions tab.

Workflow Explanation
^^^^^^^^^^^^^^^^^^^^

1. **Trigger**: Every push to the repository triggers the workflow.
2. **Environment Setup**: The workflow sets up a LaTeX distribution using the ``texlive-action``.
3. **Compilation**: The workflow runs ``pdflatex`` and ``biber`` commands to generate the PDF.
4. **Artifact Upload**: The compiled PDF is saved as an artifact in the Actions tab for easy download.

Using GitHub Actions
--------------------

1. Push your changes to the repository.
2. Wait for the GitHub Actions workflow to complete.
3. Download the compiled PDF from the Actions tab in your repository.

Workflow Configuration
----------------------

The GitHub Actions workflow is defined in ``.github/workflows/latex.yml``:

Customization
-------------

- **Adding Images**: Replace ``example-image.png`` with your own image and update the path in the ``example.tex`` file.
- **Updating References**: Add your references to the ``references.bib`` file in the proper BibTeX format.
- **Modifying Content**: Edit the ``example.tex`` file to suit your needs.

Output Example
--------------

The output document includes:

- Title page
- Table of contents
- Sections with sample text, images, tables, and equations
- Automatically formatted bibliography


License
-------

This project is licensed under the MIT License. See the ``LICENSE`` file for details.