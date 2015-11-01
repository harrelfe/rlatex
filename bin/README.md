# Executable Scripts

|*Script*|*Purpose*|
--------|--------
| `knitr` | Run R in batch mode, showing progress using the `xless` viewer (`sudo apt-get install xless`); keeps the window open until you kill it or type `ctrl-c` at the console.  Usage: `knitr foo` to process `foo.Rnw` and create `foo.tex` and graphics files |
| `knitrn` | Like `knitr` but closes `xless` window as soon as R finishes; useful if you don't expect bugs in the `.Rnw` file |
| `knitrnf` | Like `knitrn` but to run from a specified directory |

#### Installation of Scripts
On `Linux` systems, assuming `~\bin` is in your system path, run:

```
cd ~/bin
wget https://raw.githubusercontent.com/harrelfe/rlatex/master/bin/knitr
wget https://raw.githubusercontent.com/harrelfe/rlatex/master/bin/knitrn
wget https://raw.githubusercontent.com/harrelfe/rlatex/master/bin/knitrnf
chmod +x knitr knitrn knitrnf
```

Then from any directory run the needed command, e.g. `knitr myfile` ro run `myfile.Rnw` and produce `myfile.tex`.
