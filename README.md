# Object Recognition #

A python object recognition using OpenCV and Yolo3.


### What is this repository for? ###

* A simple implementation using python language
* Version 1.0

### System requirements ###
* Python 3.7
* OpenCV 3.4.10.35 (`pip3 install opencv-python==3.4.10.35`)
* NumPy 1.21.6 (`pip3 install numpy==1.21.6`)
* Computer with GPU, built-in gpu might work it will just be slow.
* Yolo3 datasets, you can download this files from Darknet repository `https://github.com/pjreddie/darknet`
	* `coco.names`
	* `yolov3.cfg`
	* `yolov3.weights`
* `git-lfs` to push yolo files.

**Note:** You can run the python library installation by using `pip` by running this on your project root directory `pip3 install -r requirements.txt`

If you want to add new library you need to --
1. Create a new branch and want to commit please run `pip3 freeze > requirements.txt` and create your own branch (see **Contribution guidelines > Branch prefix** for more details) and create pull-request merging towards `staging` branch.


### How do I get set up? ###

* Install your preferred IDE, i recommend `pyCharm`
* I also recommend the use of python virtual environment `venv`. See [Creation of virtual environments](https://docs.python.org/3/library/venv.html).
* See `requirements.txt` python library dependencies

### Contribution guidelines ###

##### Branches #####

* `main` - This is the main branch only the admin maintainer can do a merge and should be from a `staging` which most pull-request are merged into except for hotfixes.
* `staging ` - This is a pre-release branch where updates after the pull-request gets aproved by QA, this version is a copy of `main` branch this is to avoid conflict when merging.
* `devel` - This contains all development updates. This is used for testing and compatibility between updates. Requires pull-request to merge with ongoing update for testing.

##### Branch Prefixes #####
Apart from the main branches we will use branch prefix to properly organize individuals branches, this is usefull during development

* `bugfix/<issue #>-<bug short description>` - Typically used to fix Release branches.
* `hotfix/<name of hotfix>` - Used to quickly fix `main` branch without interrupting changes in the `devel` and `staging` branch.
* `feature/<name of the feature>` - Used for specific feature work or improvements. Generally branch from, and merge back into, the `staging` branch using pull requests.
* `release/<release version>` - Used for release task and long-term maintenance versions. They branch from, and merge back into, the `staging` branch.
