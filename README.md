# SayMyName

<figure align="center">
    <img src="./images/me-wlater.jpeg"/>
    <figcaption>Image Created by: <a href="https://github.com/mrakhgari/whoAreYou">WhoAreYou?</a></figcaption>
</figure>

My resume and CV.

## Pre-Build Version

Pre-build versions are available as Github Releases in PDF. Each release has build date as its name.

## Build Yourself

### Requirements

A full TeX distribution is assumed. [Various distributions for different operating systems (Windows, Mac, \*nix) are available](http://tex.stackexchange.com/q/55437) but TeX Live is recommended.
You can [install TeX from upstream](https://tex.stackexchange.com/q/1092) (recommended; most up-to-date) or use `sudo apt-get install texlive-full` if you really want that. (It's generally a few years behind.)

If you don't want to install the dependencies on your system, this can also be obtained via [Docker](https://docker.com).

#### Usage

At a command prompt, run

```bash
xelatex {your-cv}.tex
```

Or using docker:

```bash
docker run --rm --user $(id -u):$(id -g) -i -w "/doc" -v "$PWD":/doc thomasweise/texlive make
```

In either case, this should result in the creation of `{your-cv}.pdf`


## Credit
[**Awesome-CV**](https://github.com/posquit0/Awesome-CV) is LaTeX template for a **CV(Curriculum Vitae)**, **Résumé** or **Cover Letter** inspired by [Fancy CV](https://www.sharelatex.com/templates/cv-or-resume/fancy-cv). It is easy to customize your own template, especially since it is really written by a clean, semantic markup.
