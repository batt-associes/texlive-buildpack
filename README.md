# texlive-buildpack

This buildpack will install the most recent TeX Live distribution with a custom set of collections:

- collection-basic
- collection-langfrench
- collection-latex
- collection-latexextra
- collection-latexrecommended
- collection-pictures
- collection-plaingeneric

## Why

This repository was first intended to install the smallest TeX Live distribution required for
PyLaTeX to run for the desired purposes. The target platform was Scalingo where the whole app
image has to be [under 1 GiB][size-limit].

## Resources

- [TeX Live quick install][quickinstall]
  - [Profile file][profile]
- [2020 TeX Live Guide][texlive-doc]
  - [Unix][unix]
  - [Command-line][cli]
  - [Setting environment variables][env-var]

[//]: # (--- Images and links section ---)

[size-limit]: https://doc.scalingo.com/platform/deployment/limits

[quickinstall]: https://www.tug.org/texlive/quickinstall.html
[profile]: https://www.tug.org/texlive/doc/install-tl.html#PROFILES

[texlive-doc]: https://www.tug.org/texlive/doc/texlive-en/texlive-en.html
[unix]: https://www.tug.org/texlive/doc/texlive-en/texlive-en.html#x1-160003.1.1
[cli]: https://www.tug.org/texlive/doc/texlive-en/texlive-en.html#x1-280003.3
[env-var]: https://www.tug.org/texlive/doc/texlive-en/texlive-en.html#x1-310003.4.1
