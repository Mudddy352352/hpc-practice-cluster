# Practice cluster

A safe, simulated Slurm supercomputer that runs in your web browser. It is meant for learning to use a university HPC cluster before touching the real one. Nothing here connects to real hardware.

## How to use it

Open `index.html` in any modern browser (double-click it), or turn on GitHub Pages for this repository (Settings → Pages → Deploy from branch → `main`, folder `/`) to get a web link.

- **Terminal:** you start logged in to `login01`. Type commands as you would after `ssh`.
- **Guide tab:** 7 short lessons: files, modules, checking the cluster, first job, a Foldseek search, fixing a failed job, cancelling and interactive sessions.
- **Cluster tab:** live picture of the nodes and your jobs.
- **Cheat sheet tab:** common commands; click one to put it in the terminal.

One second on the page counts as one minute of cluster time. Progress is saved in the browser; **Reset practice** starts over.

## Supported commands

| Area | Commands |
|---|---|
| Files | `pwd ls cd cat head tail less grep wc mkdir touch cp mv rm nano` |
| Software | `module avail / load / unload / list / purge / spider` |
| Slurm | `sbatch squeue sinfo scancel sacct scontrol seff srun` |
| Other | `date hostname whoami quota df history clear man help` |

## Caveat

Partition names, limits and software versions are invented. Check your real cluster's user guide (including whether it uses Slurm or PBS) before your first real job.
