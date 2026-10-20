# Week 4: Batch SKAB contamination pipeline

The completed exercise processes the five synthetic SKAB-format files generated
by the supplied notebook. It saves contaminated sensor arrays locally, a
`contamination_catalog.csv`, and `week04_exercise1_plot.png`. This execution does
not represent a run on the full real SKAB benchmark.

Open `BAFAD_Week04_Exercise1.ipynb` with a Python kernel, install the dependencies
in `requirements.txt`, and run all cells from this directory. The notebook keeps
the supplied data-generation and carry-forward helper cells unchanged.

All supplied assertions passed. Additional checks verified all rows outside
anomaly windows, deterministic reruns, blackout mode, CSV round trips, clean
files with no windows, and windows touching the first and last rows. The saved
plot shows clean and injected Sensor 1 values for `4.csv`, with all three anomaly
windows shaded. The `variance` argument is used as the standard deviation, as
specified by the exercise's helper.

The notebook includes three interpretation answers and discloses AI assistance.
Generated input and contaminated array folders are excluded from Git; rerunning
the notebook recreates them from its fixed synthetic-data seeds.
