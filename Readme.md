# Empress: Systematic Cophylogeny Reconciliation Tool

Empress is a systematic cophylogeny tool under duplication-transfer-loss model. 

Empress was developed by students at Harvey Mudd College and was supported by 
grant 1905885 from the National Science Foundation to Harvey Mudd College. 

[The Empress website](https://sites.google.com/g.hmc.edu/empress/) has tutorials and a detailed explanation of the software.

Installation instructions are on the [Download and Run Empress Application](https://github.com/ssantichaivekin/empress/wiki/Download-and-run-empress-GUI-executables-for-macOS,-Linux,-Windows) wiki page.

If you want to help develop empress or run empress from the command line see the [Home](https://github.com/ssantichaivekin/empress/wiki) wiki page.

Tool forked from github (https://github.com/ssantichaivekin/empress.git)

```bash
git clone https://github.com/WiscEvan/empress.git
cd empress
chmod +x empress_cli.py
mamba env create --file=environment.yml
workon empress
```

```bash
usage: empress_cli.py [-h] {cost-regions,reconcile,histogram,cluster,p-value,tanglegram} ...

Empress tool for duplication-transfer-loss maximum parsimony reconciliation.

positional arguments:
  {cost-regions,reconcile,histogram,cluster,p-value,tanglegram}
                        Commands empress can run
    cost-regions        find cost regions that give same maximum parsimony reconciliations
    reconcile           find maximum parsimony reconciliations given duplication, transfer, and loss costs
    histogram           find pairwise distance histogram of all reconciliations given duplication, transfer, and loss costs
    cluster             find clusters of reconciliations with similar properties given duplication, transfer, and loss costs
    p-value             test the hypothesis that the optimal reconciliation cost was obtained using a random mapping
    tanglegram          view a tanglegram which shows the tip mapping between the two trees

options:
  -h, --help            show this help message and exit

Show help for each command by running `python empress_cli.py <command> --help`
```
