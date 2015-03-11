
# Spatial Data Analysis with PySAL

**[Sergio Rey][Rey]**



**SciPy 2015, Austin, Texas**

## Tutorial Description

A unique feature of this tutorial is the use of Python based software tools for spatial data analysis. Python is an object oriented scripting language that is gaining rapid adoption in the scientific computing and data science communities. To facilitate its adoption within the GIScience community, project founders Rey and Anselin have collaborated on the creation of [PySAL]: Python Library for Spatial Analysis. Since its initial release in July 2010, PySAL has been downloaded over 50,000 times and is now included in well- known open source scientific data analysis distributions, such as Anaconda. This tutorial will introduce participants to the latest version of PySAL (1.9.1).

This tutorial will cover the following aspects of spatial data analysis

- Reading different sources of vector based spatial data
- Visualization and mapping using PySAL with folium, CartoDB, and related packages
- Construction and manipulation of spatial weights
- Testing for spatial clustering using global spatial autocorrelation statistics
- Identification of hot and cold spots using local spatial autocorrelation statistics
- Exploratory space-time data analysis with PySAL 

## Prerequisites

- Previous experience with Python programming is recommended
- Participants should bring their own laptops to the workshop
- Software should be installed prior to traveling to the workshop (instructions below)

### Software Requirements

For the workshop we will require the following packages be installed

- PySAL 1.1.1
- SciPy
- Numpy
- iPython Notebook 2.1+
- folium

There are a number of ways to install PySAL and these dependencies. For the workshop, if you do not yet have the dependencies installed we suggest using one of two scientific Python distributions (below). These have the advantages of including most of the dependencies for PySAL as well as PySAL itself. Moreover, both allow for updating PySAL to the most recent release  (1.9.1 released January 31, 2015) which is more current that what is listed in either distribution. Both of these distributions also allow for installation of our final dependency, folium.

#### PySAL via Anaconda Python Distribution

1. Install [Anaconda Python Distribution Version 1.8.0][Anaconda]
2. Open a terminal (Mac or Linux) or Powershell (Windows)
2. `pip install -U pysal`
3. `pip install -U folium`

#### PySAL via Enthought Canopy
Note that the Academic version of Canopy comes with PySAL version 1.7. For this workshop we will be using PySAL 1.8. Upgrading in Canopy can be done as follows:

1. Install [Canopy][Canopy]
2. Run Canopy
3. From the menu select `Tools Canopy Terminal`
4. `pip install -U pysal`
5. `pip install -U folium`



#### Testing Your Installation

Once you have installed all the dependencies, you can check to confirm everything is ready to go.

For Anaconda:

1. Open a terminal (Mac or Linux) or Powershell (Windows)
2. `ipython notebook`
3. In the browser click `New Notebook`
3. In the first cell in the notebook enter  
   `import pysal`

   `pysal.version`
   
   Then `<Shift-Enter>` (i.e., hit the Shift then the Enter Key)
4. In the second cell in the notebook enter  
   `import folium`

   Then `<Shift-Enter>`
 
Your screen should look something like:
![Anaconda setup](esda/figures/anaconda.png)


For Enthought Canopy:

2. Run Canopy
3. From the menu select `Tools Canopy Terminal`
2. `ipython notebook`
3. In the browser click `New Notebook`
3. In the first cell in the notebook enter  
   `import pysal`

   `pysal.version`
   
   Then `<Shift-Enter>` (i.e., hit the Shift then the Enter Key)
4. In the second cell in the notebook enter  
   `import folium`

   Then `<Shift-Enter>`
 

Your screen should look something like:
![Enthought setup](esda/figures/enthought.png)


#### Issues

If you run into any problems, double check that you have installed both the upgraded version of PySAL and folium (see above). If problems persist, please contact me <sjsrey@gmail.com>.


[PySAL]: http://pysal.org
[GeoDaSpace]: https://geodacenter.asu.edu/software/downloads/geodaspace
[Anaconda]: http://continuum.io/downloads.html
[Canopy]: https://www.enthought.com/store
[VirtualBox]: https://www.virtualbox.org/wiki/Downloads
[VirtualBox 4.3.12]: http://download.virtualbox.org/virtualbox/4.3.12/VirtualBox-4.3.12-93733-Win.exe
[Vagrant]: http://www.vagrantup.com/downloads.html
[Vagrantfile]: Vagrantfile
[Rey]: https://geoplan.asu.edu/people/sergio-j-rey
