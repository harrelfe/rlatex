# rlatex
### `LaTeX` Packages and Templates Especially for Use with `R` and `knitr`

The `templates` directory contains templates for using the `LaTeX` packages provided here as well as `knitr` in general.

The `examples` directory contains `knitr` documents (`.Rnw`) that show how to use `LaTeX` with `R`, and also contains `.pdf` files with the output.

The `packages` directory contains the `LaTeX` package source files.  The following describes the purpose of each package there.

The `bin` directory contains `Linux/Unix` shell command helper scripts, e.g., `irlatex` for downloading from this site the latest versions of the packages and installing them in the central location for `LaTeX` add-on packages.

|*Package*|*Purpose*|
--------|--------
| `hslide.sty` | Documents that double as handouts and slides, using `knitr` |
| `knitrl.sty` | For use with `knitr` allowing pretty-printing and minimal but effective framing of `R` code and output, replacing `Sweavel.sty` |
| `spaper.sty` | Statistical reports + manuscript composition handling author comments/todo lists |
| `hbeamer.sty` | Beamer presentations for use with `knitr` |

See also [greport.sty](https://github.com/harrelfe/greport/blob/master/inst/greport.sty) and [here](http://biostat.mc.vanderbilt.edu/BiostatisticianResponsibilities).


#### Installation of `LaTeX` Packages
On `Linux` systems using `TeXLive`, run the following `bash` script to install the `irlatex` `bash` script stored here.  Make sure that `~/bin` is in your system path.

```
cd ~/bin
wget https://raw.githubusercontent.com/harrelfe/rlatex/master/bin/irlatex
chmod +x irlatex
```

Then from any directory run the command `irlatex` which will download and install in your personal central `LaTeX` package system all of the packages stored here.

To find out where to put add-on `LaTeX` packages, at the command line type
```
kpsepath tex | tr : '\n'
```
and see which paths end in two or three slashes.  That way you will not need to run the `mktexlsr` program if you update the local styles.  Pick a directory that is in your home area if you want to keep things simple.  `irlatex` assumes `~/texmf/tex`.
