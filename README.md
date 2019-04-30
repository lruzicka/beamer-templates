# How to use Fedora Presentation Template

The Beamer template is defined by several **style files** (*.sty*), these are:

1. `beamertheme*.sty`

2. `beamerinnertheme*.sty`

3. `beameroutertheme*.sty`

4. `beamercolortheme*.sty`

In this repository, there are two directories called `fedora43` and `fedora169` that hold settings for different slide ratios, such as 4:3 and 16:9. They include the above files. You can see, that the file names also have an addition where the asterisk is put in the above list. For 4:3 ratio, the files use another `Fedora` addition, while for 16:9 they use `Fedora169`.

## Using the 4:3 ratio in your presentation.

### Prerequisites

1. Copy the **style files** (`beamerthemeFedora.sty` and others) to a directory where you want to build your Beamer presentation.

2. Copy the `sidebar.png` and the `titlepage43.png` to the same directory.

3. Install additional packages for your **Texlive** distribution:

   1. Install the font package (`texlive-montserrat`).

   2. Install the **ly1** package (`texlive-ly1`).

Now, you can start working on your presentation in Beamer.

### Beamer preambule settings

There are some requirements, that you have to set in the preambule (Beamer header), so that Beamer would use the templates correctly. Check one possible working preambule:

---

\documentclass[12pt]{beamer} % Setting different fontsize will break the template.
\usepackage[utf8]{inputenc} % Support for UTF-8.
\usepackage[T1]{fontenc} % Support for T1 fonts.
\usepackage{lmodern}
\usetheme{Fedora} % Loads the Fedora template.
\usepackage{graphicx} % If you want graphics.
\usepackage{montserrat} % Fedora presentation font

---

## Using the 16:9 ratio in your presentation.
