# Snakemake tutorial with data

This repository hosts the final code and data needed for the [Snakemake tutorial](https://snakemake.readthedocs.io/en/stable/tutorial/tutorial.html).


Run in VScode using binder:  [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/enryH/snakemake-tutorial/master?urlpath=vscode/?folder=/home/jovyan/snakemake-tutorial-data)
(refresh if you get at 500 error code)

## To try

```bash
snakemake --help
snakemake -n # --dryrun
snakemake -n - # --printshellcmd
snakemake --cores 1 # execute locally with N cores
snakemake --report report.html # after running snakemake, create a report
snakemake --dag | dot -Tpng > dag.png # look at directed acyclic graph (DAG) of jobs 
snakemake -n --forceall # force re-run, otherwise everything was done
snakemake --forceall --use-conda --conda-frontend mamba # run with newly create environments
snakemake --print-compilation > snakemake.py # inspect python script generated based on Snakefile
```

### Questions/Topics raised
- explain what wildcards of a rule are
- tutorial is a simple read-alignment pipeline
- What are ancient, temp, pipe statements etc around file names


If you want to revert changes with the possibility to replay them, use 
[`git stash`](https://git-scm.com/book/en/v2/Git-Tools-Stashing-and-Cleaning)
```bash
git stash --all
```

## CHANGELOG

- png instead of svg histogram (easier to view)
- latest code-server  (`4.5.0`) is not working with mybinder
