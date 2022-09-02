# Vapor Visualization Tutorial

Hi! This repository includes the Jupyter notebooks we'll reference during the tutorial, as well as a few how-to docs. Note that I have already prepared Vapor-readable data in advance, but I also want to show you how to create such files. During the tutorial, we'll focus on the data I've prepared using `VAPOR_Visualization.ipynb` and `nco.md`, and then we'll use `automate_example.ipynb` to make an animation of our Vapor renderings. 

In this repository, you'll find:

1. `VAPOR_Visualization.ipynb`: This Jupyter Notebook demonstrates how to pull variables from a Bifrost simulation, how to calculate a few secondary variables, and how to write that information into a netCDF file that is CF-compliant and readable in Vapor

2. `automate_example.ipynb`: This Jupyter Notebook demonstrates how to write a tailored automation script using pyautogui, which is super helpful when your Vapor commands get repetitive. Then, the script uses imagio and moviepy to create an animation (both gif & mp4) out of the snapshots taken in Vapor

3. `nco.md`: This is a how-to on post-processing netCDF files after they're written

4. `python_dependencies.md`: This is a list of python packages that are necessary for `automate_example.ipynb`

## Where can I find the already-prepared data?

Check here, and download everything here to your local machine: `/mn/stornext/d18/RoCS/rebecrob/tutorial_data`
