# A Brief Primer on X-ray Diffraction Crystallography

At the time of writing this project, I am a student in the Department of Physics in Scottish Church College, Kolkata, India, pursuing the B.Sc. Physics (Honours) program under the University of Calcutta.
I will be submitting this project for the *tutorial* portion in the Discipline Specific Elective course "Nano materials and Applications" in Semester 6.

**Update:** The project has been formally submitted on 12 May 2023.

## Please note:

 - This is a project and **not** a B.Sc. thesis or dissertation.
 - I have compiled the files using `LuaLaTeX`. If you would like to get the same output as mine, please use the same engine. Compatibility is not guaranteed on other engines.
 - The fundamental structure of the document is based on the publication style in the Journal of High Energy Physics. The `jheppub.sty` file takes care of this, and it has been downloaded from the journal website, with a few modifications made by me.
 - JHEP uses `natbib` with `BibTeX`, which is the standard in most journals. I wanted to go with `BibLaTeX`, however. Hence, I have modified the `jheppub.sty` file to not import the `natbib` package.
 - Some bibliographic entry types like `@online` are only available in `BibLaTeX`. Hence, the bibliography file will need editing if `BibTeX` is to be used.
 -  `biber` has been used as the backend to `BibLaTeX`.

## Building the PDF file

The master document is `main.tex`.

To compile the PDF, please follow these steps:

 - Clone the repo. Since a lot of images are also indexed in git, you may like to only clone the latest commit on the `main` branch using:
 
 ```bash
 git clone --depth=1 <repo_url>
 ```
 
 - Execute `LuaLaTeX` and `biber` in the followng order:
    - `LuaLaTeX` ✕  1
    - `biber` ✕  1
    - `LuaLaTeX` ✕  3 (or 4)

Building a proper bibliography requires at least two compilations with `LaTeX` after running `biber`. A third iteration is necessary to properly compile the `tikz` diagrams. A fourth iteration may be needed if there are spurious green lines on some pages.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" width="200" src="https://mirrors.creativecommons.org/presskit/buttons/88x31/png/by-nc-sa.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

## Contribution Guidelines

As mentioned before, this is a project. Therefore, once submitted, the main material of this repo will be frozen, and issues and PRs changing the content will not be entertained. You are, of course, free to clone the repo and make changes to anything and everything in accordance with the terms of the license. PRs fixing any typesetting bug will be looked into, however, as long as it does not change the basic structure of the document (you cannot, for example, change the document class, remove the `jheppub.sty` package or port to `BibTeX` in a pull request).
