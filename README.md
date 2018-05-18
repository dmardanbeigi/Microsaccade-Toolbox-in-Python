# Microsaccade-Toolbox-in-Python
A python implementation for extracting microsaccades in python based on the algorithm proposed by Engbert et al. (2006). 

The microsaccades are extracted seperatly for the left and the right eye and binocular microsaccades are then detected by a temporal overlap criterion on the left and the right results. 
Monocular microsaccades are filtered based on the amplitude, duration and peak velocity criteria defined by the user.
A secondary step of filtering will be applied on the remaining candidates based on the RANSAC linrear regression on the main sequence and all the outliers will be removed based on this. 

![](https://github.com/dmardanbeigi/Microsaccade-Toolbox-in-Python/blob/master/Screen Shot.png)
![](https://github.com/dmardanbeigi/Microsaccade-Toolbox-in-Python/blob/master/MainSequence.png)


## Getting Started

All the main functions are defined inside the file "functions.ipyn" and the notebook file "Microsaccade Toolbox for Python.ipynb" contains examples of the things you can do with this toolbox. 

## Requirements

You need python 3.7 and a few necessary libraries.

### Installing
Installation instruction for Mac (would be similar for windows):
1- Download and install python 3.6.x from https://www.python.org/downloads/
Mac:
2- Open the terminal (find the Terminla in \Applications\Utilities\terminal)
3- Go to the project folder from your terminal:
cd <path to your installation folder 
4- run the following lines:
pip3 install -r requirements.txt
jupyter contrib nbextension install --user

## Authors

* **Dr. Diako Mardanbegi** <dmardanbeigi@gmail.com>
http://www.dmardanbegi.com

## License

This project is licensed under the terms of the GNU General Public License.

## Acknowledgments
* [Engbert et al. (2015) Microsaccade Toolbox for R](http://read.psych.uni-potsdam.de/index.php?option=com_content&view=article&id=140:engbert-et-al-2015-microsaccade-toolbox-for-r&catid=26:publications&Itemid=34
)
* Engbert, Ralf. "Microsaccades: A microcosm for research on oculomotor control, attention, and visual perception." Progress in brain research 154 (2006): 177-192.
