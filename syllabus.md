# Intro to training 
(Yoshi Tamori)
* Installation
	- check installation: local or docker 
	- check who knows what
        - I think you should add this part :):) Carlos. 
        - This modification is going to branch_1.

* p-value questionnaire
		[Start here](http://www.reproducibleimaging.org/module-stats/03-p-values/)
* Get better at 
	- python
		[Here is a good start for python](https://neurohackweek.github.io/python-for-programmers/)
	- Git/github
		[From NHW](https://github.com/neurohackweek/git-and-github)
	- numpy, stats module in scipy, matplotlib
		[numpy from nipype workshop](http://nbviewer.jupyter.org/github/nipy/workshops/blob/master/170327-nipype/notebooks/numpy-advanced/numpy_advanced_py3.ipynb)
		[scipy.stats]()
	- know the existence of other higher level modules:
		[a superbe resource here](http://www.scipy-lectures.org/packages/index.html)
		- Pandas
		- statmodels
		- scikit-learn
		- bayesian modules
* Issue: diverse students
* Time is short
* Solution: rapid overview of things, then projects

Project 1: basic stats
.......................
	1) check that a p-value is uniformly distributed 
	2) why is the estimation of effect size over estimated in the literature ? implement a demonstrator of the problem. What affects this over estimation?

Project 2: More involved
.........................
	1) Take the PING dataset
	2) Investigate the effect of Sex depending on the counfounds included in the model (eg site, SES, etc) 

Project 3: Non parametric version of a power analysis
.......................................................
	1) Consider that there is a dataset available that is close enough to 

Project 4: construct a p-hacking test
.........................................
	1) suppose you have a set of p-values from your literature
	2) construct a X2 test  

Project 5: scikit-learn ? 
...........................
	- try to see if prediction analysis is more resilient to choice of cohort than p-value



# Material / Docker commands 

## linux & OSX
cd ~
mkdir docker-data
Linux: docker run -it --net=host -v ~/docker-data:/repos  satra/sfn-17:0.5
OSX: docker run -it -v ~/docker-data:/repos  satra/sfn-17:0.5

## Windows
#### create in your home directory "docker-data"

docker run -it -v C:\{username}\docker-data:/repos  satra/sfn-17:0.5

# Inside docker

cd /repos
git clone  https://github.com/ReproNim/module-stats.git
cd module-stats/notebooks
ls
jupyter notebook --ip=* --port=9999 Positive-Predictive-Value.ipynb

## On Windows: 
- instead of “localhost”, run “docker-machine.exe ip” to get your docker machine IP address.  
Then use this in place of “localhost”

<<<<<<< HEAD
changed by H.Ikeno

change change change
test
=======
# GIT tutorial. Alexander Woodward
>>>>>>> ea551992866503305df467b6807459867165820b
