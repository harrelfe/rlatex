# rlatex
### `LaTeX` Packages and Templates Especially for Use with `R` and `knitr`

The `templates` directory contains templates for using the `LaTeX` packages procided here as well as `knitr` in general.

The `examples` directory contains `knitr` documents (`.Rnw`) that show how to use `LaTeX` with `R`, and also contains `.pdf` files with the output.

The `packages` directory contains the `LaTeX` package source files.  The following describes the purpose of each package there.

The `bin` directory contains `Linux/Unix` shell command helper scripts, e.g., `irlatex` for downloading from this site the latest versions of the packages and installing them in the central location for `LaTeX` add-on packages.

|*Package*|*Purpose*|
--------|--------
| `hslide.sty` | Documents that double as handouts and slides, using `knitr` |
| `knitrl.sty` | For use with `knitr` allowing pretty-printing and minimal but effective framing of `R` code and output, replacing `Sweavel.sty` |
| `spaper.sty` | Statistical reports + manuscript composition handling author comments/todo lists |

See also [greort.sty](https://github.com/harrelfe/greport/blob/master/inst/greport.sty).


#### Installation of `LaTeX` Packages
On `Linux` systems using `TeXLive`, run the following `bash` script to install the `irlatex` `bash` script stored here.  Make sure that `~/bin` is in your system path.

```
cd ~/bin
wget https://raw.githubusercontent.com/harrelfe/rlatex/master/bin/irlatex
chmod +x irlatex
```

Then from any directory run the command `irlatex` which will download and install on your central `LaTeX` system all of the packages stored here.



