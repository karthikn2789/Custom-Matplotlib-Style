## Creating custom Matplotlib style

This repository consists of two Jupyter notebooks to demonstrate how to create and use custom styles in Matplotlib. The first notebook [Data_Visualisaton_Example](Data_Visualization_Example.ipynb) customises three sample graphs using matplotlib's inline customisations. The main drawback here is that these customisations must be applied to every graph in a project. This can be overcome by creating a .mplstyle file which holds all the needed customisations in a single place. The repository consists of two .mplstyle files with varying levels of customisations.

The second notebook, [Data_Visualisation_Example_with_mplstyle](Data_Visualization_Example_With_mplstyle.ipynb) does the same customisations as the previous notebook with one difference. It makes use of [demo_style.mplstyle](demo_style.mplstyle) file to customise its graphs. The key advantage here is that you just need to add line of code instead of adding customisations to every graph. The line `plt.style.use(demo_style.mplstyle)` is all it takes to instruct Matplotlib to use this file for applying customisations to all the graphs in a given Jupyter notebook or a python script.

A couple of comparisons between Matplotlib's styles and a custom [demo_style_2.mplstyle](demo_style_2.mplstyle).

![All vs custom wave](../all_vs_demo2_wave.png)
![All vs custom bar](../all_vs_demo2_bar.png)

If you wish to change the style of a single graph or chart while using .mplstyle, you can always override the custom style using inline customisations. Using inline customisation does not affect the .mplstyle file and the customisation will apply only to that graph or chart.