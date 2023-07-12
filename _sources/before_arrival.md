# Before you arrive

Although the colloquium does not require a signficant amount of preparation before the meeting, it would help students get the most out of the colloquium if they were to familiarize themselves with as many of the items below as possible.

This is not meant to be exhaustive at this time. But If anything is unclear, doesn't work, or you need further help, please contact [Rich Neale](mailto:rneale@ucar.edu). I hope to set up a messaging group for us all (either Google chat or Slack) and will send out survey questions about that and a few other topics also.


## Computing requirements and setup

The colloquium will operate under the assumption that students have a working laptop available to them for the entire 2 week period. A mac or windows machine is preferable. The most recent updates of software should be applied where possible. Please contact [Rich Neale](mailto:rneale@ucar.edu) as soon as possible if you are unable to provide a laptop of your own.


Priority software that should be installed (or updated) and available on your laptop: 

* Conda ([Download](https://docs.conda.io/en/latest/miniconda.html): windows/mac/linux)
	* This will allow us to a import and use a number of packages below, especially related to using python
* [github](https://github.com/)
	* github is a widely used code revision software for large code bases that are collaboratively developed 
	* You will need to sign up if you do no currently have a log in. It's pretty simple and we'll use it only for a few downloads of data from the collqouuim repository
	* It is easily installed using conda: `conda install -c conda-forge git`
* [Python](https://www.python.org/)
	* This software comes with the conda install by default
	* It is the analysis and plotting software that most people will be familiar with. We will provde some minimal diagnostics scripts, but hope that students develop (and possibly share) their own scripts with others.
	* As an example here are simple plotting guidelines from the [CESM tutorial](https://ncar.github.io/CESM-Tutorial/notebooks/diagnostics/cam/basics.html)
	* Key to using the correct packages in a notebook (e.g., [`xarray`](https://docs.xarray.dev/en/stable/) - which handles multidimensional arrays) is the creation of conda environments ([example](https://medium.com/@nrk25693/how-to-add-your-conda-environment-to-your-jupyter-notebook-in-just-4-steps-abeab8b8d084)). See if you can create and use an environment in jupyter-hub from this example.
	
* [jupyter-hub](https://jupyterhub.readthedocs.io/en/stable/#)
	* Jupyter-hub is a web-based server that can handle simple file editing, ssh sessions to the NCAR supercomputers and editing of python and jupyter notebooks that streamline analysis of data. 
	* It can easily be installed as a conda package: `conda install -c conda-forge jupyterlab`

* A commonly used web browser (e.g., chrome, firefox, safari)
	* This is needed for both your local (laptop) jupyterhub server and the NCAR machines ([Cheyenne](https://arc.ucar.edu/knowledge_base/70549542) and [Casper](https://arc.ucar.edu/knowledge_base/70549550)) jupyter-hub server. The NCAR [jupyter-hub server](https://jupyterhub.hpc.ucar.edu/) will be ready to use when you get your CISL login credentials (see below)

* Some alternatives to jupyterhub for connecting to [Cheyenne](https://arc.ucar.edu/knowledge_base/70549542) and [Casper](https://arc.ucar.edu/knowledge_base/70549550) and file editing
	* Terminal clients ([mac](https://www.makeuseof.com/best-ssh-clients-mac/)|[windows](https://www.maketecheasier.com/best-terminal-emulators-for-windows/))
	* Text Editors: emacs ([mac](https://emacsformacosx.com/)|[windows](https://www.gnu.org/software/emacs/download.html)) or vi ([download](https://www.vim.org/download.php))

## NCAR Supercomputer Environment

To run both WRF and CESM access will be made available to students on the NCAR [Computational Information Systems Laboratory (CISL)](https://www2.cisl.ucar.edu/) supercomputing environment. This will include the NCAR-University Wyoming supercompute [Cheyenne](https://arc.ucar.edu/knowledge_base/70549542) and compute cluster [Casper](https://arc.ucar.edu/knowledge_base/70549550). You will receive information about your usernames on the CISL systems soon (hopefully by July 3). Once you have received your credentials you should try to [**access the system and setup your user space software**](https://arc.ucar.edu/knowledge_base/74317885)

## Reading material
There is a wide array of material available for learning about and understanding atmospheric boundary layer science (both free and for purchase). A couple of classic books to be maybe dip into over the next 2 weeks if you have lots of time are [An Introduction to Boundary Layer Meteorology (Stull)
](https://link.springer.com/book/10.1007/978-94-009-3027-8), [Fundamentals of Boundary-Layer Meteorology](https://www.amazon.com/Fundamentals-Boundary-Layer-Meteorology-Springer-Atmospheric/dp/3319608517) and [Atmospheric Boundary Layer: Integrating Air Chemistry and Land Interactions](https://www.cambridge.org/core/books/atmospheric-boundary-layer/5DAB600E63724FF20543CFD5E29FE237). Of course these books are very expensive if your librbary does not have a copy. However, there are also many sets of excellent university course notes available that make good reading, e.g., [University of Washington (Chris Bretherton)](https://atmos.uw.edu/~breth/classes/AS547/), great introcuction to theory) and [University of British Columbia](https://www.eoas.ubc.ca/books/Practical_Meteorology/prmet102/Ch18-abl-v102.pdf), great visuals of boundary layer morphology.


## Presentations

As a 'get to know everyone' on the first day of the colloquium (Monday 17th July, 11-12:30) we are asking each of you to give a 3 minute presnentation using 2 slides only. We would like you to spend the first slide talking generally about your graduate project (topic, hypotheses, key findings if you have them). Remember that each student is at a different  stage in their research, and it's not meeant to be a test in any way. For the 2nd slide we would like you to talk about a recent problem you had tried to address very recently (~weeks). You could have been successful or not at solving it! The aim is that students get a sense of other students' day to day activities. So think about the content and be sure to drop your slides in [this google drive]() that everyone should have access to. Email me if not!

On the final afternoon (Friday, 28th July) we ask the students to give a 5-minute summary presentation of their findings from the research they worked on during the project time of the colloquium. The goal is not only to communicate your ideas but also stimulate conversation wih the rest of the group on how the research project could be carried forward. There is a [student google folder]() available and we request that students upload their 'get to know everyone' slides (2 max) by the 16th July if possible.


## Community Earth System Model (CESM)
Another option is the the [Community Earth System Model (CESM)](https://www.cesm.ucar.edu/). CESM is a global climate model supported at NCAR and has multiple climate applications including common [CMIP type applications](https://www.wcrp-climate.org/wgcm-cmip) as well as [as earth system prediction](https://www.cesm.ucar.edu/working-groups/earth-system). For the colloquium we will perform experiements in a simplified AMIP configuration that prescribe Sea Surface Temperatures and this focus primarily on the [Community Atmosphere Model (CAM)](https://www.cesm.ucar.edu/models/cam). In terms of representing boundary layer processes CAM uses the high order Cloud Layers Unified By Binormals (CLUBB) parameterization scheme. It is a somewhat complex scheme, but has numerous degrees of freedom that enable a wide variety of sensitivity experiments to be performed. If you are unfamiliar with CESM and are interested in using this model during the colloquium, please familiarize yourself as much as you can with the model [here](https://www.cesm.ucar.edu/models/cam). We will go over the fundamentals of running the model during the coloquium, but the [CESM Tutotial webages](https://ncar.github.io/CESM-Tutorial/README.html) will give you a more comprehensive workflows that the model uses. And finally if you are interested in an initial understanding of CLUBB


## Weather Research and Forecasting Model (WRF)

For a more weather event based study exercise using the [Weather Research and Forecasting Model (WRF)](https://www.mmm.ucar.edu/models/wrf) will be available. WRF is a forecast capable model that can simulate past weather events over a limited area of the globe. Unlike CESM multiple boudary layer parameterization options are available which allows you to perform sensitivity experiments to investigate the assumptions use in different options and how they impact specific weather events.
We will go over the fundamentals of running WRF in the collqouium, but feel free to familiarize yourself with methods for [running WRF](https://www2.mmm.ucar.edu/wrf/users/) in advance.

## Chemistry Land-surface Atmosphere Soil Slab (CLASS) model

For a simpler model that has a focus more on chemical processes we will be using the [Chemistry Land-surface Atmosphere Soil Slab model (CLASS)](https://classmodel.github.io/). CLASS is a model that can be downloaded and run easily on a laptop. The instructions for downloading onto a windows or mac system are [here](https://github.com/classmodel/modelgui/releases). A series of comprehensive introductory [videos](https://classmodel.github.io/clips.html) can be viewed here. Try to download and have a play with the easy to use interface.







