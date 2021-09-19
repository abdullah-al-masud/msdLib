<h1>
  msdlib
</h1>
<br>

<img src="msdlib_logo_fit.png" alt="msdlib_logo" width="150"/>

![](https://img.shields.io/pypi/l/msdlib.svg)
![](https://badge.fury.io/py/msdlib.svg)
![](https://travis-ci.org/abdullah-al-masud/msdlib.svg?branch=master)
![](https://readthedocs.org/projects/pip/badge/?version=latest)

![](examples/plot_time_series_example/Combined_Time_Series_Plot.jpg)



<h2>
Introduction
</h2><br>
The main purpose of this library is to make data science works easier and simpler with less amount of coding, providing helper functions for plotting, 
ML training, evaluation, result summarization etc. 
The purpose is to focus more on making common tasks easier so that a beginner to mid level developer is able to do his/her jobs easily and can get started career with enough pace.<br><br>



<h2>
Dependencies
</h2><br>

* Numpy
* Pandas
* Matplotlib
* Scipy
* Seaborn
* joblib
* Pytorch

All of these packages except Pytorch will be installed automatically during msdlib installation.

Pytorch should be installed by following installation procedure suggested https://pytorch.org/.<br><br>



<h2>
Installation
</h2><br>

``pip install msdlib``

or if you have --user related issues during installation, please use

``pip install --user msdlib``
<br><br>


<h2>
License
</h2><br>
MIT open source License has been issued for this library.<br><br>



<h2>
Examples
</h2><br>
You can find easy examples on how to use the functions and classes from this library `here <https://github.com/abdullah-al-masud/msdlib/tree/master/msdlib/examples>`_.
Necessary data is also provided in this directory.<br><br>



<h2>
Documentation
</h2><br>
Complete documentation of classes and functions can be found here https://msdlib.readthedocs.io/.
<br><br>


<h2>
Reference/citation
</h2><br>

```
@manual{msdlib,
title        = "{msdlib}: A package for easier data science practices",
author       = "{Abdullah Al Masud and {msdlib Developers}}",
month        = Jan,
year         = 2020,
url          = "{https://github.com/abdullah-al-masud/msdlib}"
}
```
<br><br>


<h2>
Call for contributions
</h2><br>

We seek active participation of enthusiastic developers from around the world to enrich this library more, adding more functionalities from different aspects,
giving more flexibility, completing unfinished functionalities and maintain the library in regular manner. 
We would be grateful for your invaluable suggestions and participations.
<br><br>


<h2>
Overview
</h2><br>

The whole library can be divided into 4 main portions.

1. Machine learning tools
2. Visualization tools
3. Data processing tools
4. Fintech and Miscellaneous


Some of the frequently used programs are shown bellow.
<br><br>

<h3>
1. Machine Learning Tools
</h3><br>
<br><br>

<h4>
mlutils:
</h4>
This module provides functionalities for easier implementation of Pytorch Deep Learning models. It offers several facilities such as-

    * Scikit-like easy implementation of Pytorch models using fit, predict and evaluate methods
    * Constructing Deep Learning models in a few lines of code
    * Producing automated results with beautiful tables having precision, recall, f1_score, accuracy and specificity in classification problems
    * Producing automated graphs of true-vs-prediction and result preparation for regression model
<br><br>


<h4>
paramOptimizer:
</h4>
This is a class which can conduct easy Hyper-parameter optimization process. 
Currently it enables us to apply grid search and random search for any model/function/mathematical entity
<br><br>


<h4>
SplitDataset:
</h4>
This is one of the most useful classes in this library. It enables us to split data set into train, validation and test sets. 
We have three options here to split data set-

    * random_split
    * cross_validation_split
    * sequence_split (specially necessary for RNN/LSTM)
<br><br>


<h4>
one_hot_encoding: 
</h4>
This function converts classification labels in one hot encoded format
<br><br>


<h4>
feature_evaluator:
</h4>
This function is one of the most useful tools. It can calculate feature importance from statistical point of view. 
It can show the results using bar plot and can handle classification and regression both kind of labels.



<h4>
class_result: 
</h4>
This function calculates classification model evaluation parameters like precision, recall, accuracy, f1 score, specificity etc. and also able to show confusion matrix as a pandas dataframe.
<br><br>


<h4>
rsquare_rmse: 
</h4>
This function calculates r square value and root mean square error.
<br><br>


<h3>
2. Visualization Tools
</h3><br>


<h4>
data_gridplot:
</h4>

![](examples/data_grid_plot_example/Grid_plot_for_Iris_dataset.jpg)

Its a function for scatter plots between every pair of features along with distributions (similar to matrix_plot in pandas). But it enables you to save the image, change figure_size, titles etc and also has one special feature for clusters in the data if any.
<br><br>


<h4>
plot_time_series:
</h4>

![](examples/plot_time_series_example/Combined_Time_Series_Plot.jpg)

This is a function and the most useful function for me from all my library functions and classes. It helps to plot time series data with a lot of flexibility. Please check out the example scripts for illustrations and guidance to use it.
<br><br>


<h4>
plot_heatmap:
</h4>
Flexible heatmap plotter function with options to remove symmetrical triangular side and many other options.
<br><br>


<h3>
3. Data Processing Tools
</h3><br>



<h4>
Filters:
</h4>

![](examples/filters_and_spectrogram_example/recorded_signal.jpg)
![](examples/filters_and_spectrogram_example/filter_spectrum.jpg)
![](examples/filters_and_spectrogram_example/Frequency_Spectrum_of_filtered_stereo_1.jpg)
![](examples/filters_and_spectrogram_example/filtered_stereo_1_with_bp_filter_with_cut_offs_[1800._2500.].jpg)
![](examples/filters_and_spectrogram_example/Spectrogram_of_stereo_1.jpg)
![](examples/filters_and_spectrogram_example/Spectrogram_of_filtered_stereo_1.jpg)

This is a class defined for applying low pass, high pass, band pass and band stop filters. It also enables us to visualize frequency domain of the signal, designed filter and also let us visualize the filtered signal if we apply a filter on the signal.
<br><br>


<h4>
get_spectrogram:
</h4>

![](examples/filters_and_spectrogram_example/Spectrogram_of_stereo_1.jpg)

This is a function that allows us to calculate spectrogram of any time series signal and also plots heatmap for that spectrogram with proper frequency bins and time axis.
<br><br>


<h3>
4. Fintech & Miscellaneous
</h3><br>



<h4>
msdbacktest (under development):
</h4>
This module intends to provide helper functionalities for trading automation, strategy implementation, back-testing, 
evaluating strategy by different popular ratios like maximum drawdown, calmar ratio, sharpe ratio etc.
Currently only a few functionalities are available and is still under development.
<br><br>


<h4>
ProgressBar:
</h4>
This is a custom progress bar which shows loop progress with a visual bar along with other information like elapsed and remaining time, loop count, total count, percentage of completion etc. (You should only use it if you dont print anything inside your loop)
