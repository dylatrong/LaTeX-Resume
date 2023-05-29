### Intro

A single-page, one-column resume for software developers. It uses the base latex templates and fonts to provide ease of use and installation when trying to update the resume. The different sections are clearly documented and custom commands are used to provide consistent formatting. The three main sections in the resume are education, experience, and projects. This project is a fork of [sb2nov's LaTeX resume project](https://github.com/sb2nov/resume).

### Build using Docker

```sh
# Pull the latest Miktex image.
docker pull miktex/miktex

# Create a volume for Miktex to work with.
docker volume create --name miktex

# Compile the tex file to PDF.
docker run -ti -v miktex:/miktex/.miktex -v ${PWD}:/miktex/work miktex/miktex pdflatex 'Resume.tex'

```


