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
	* `yolov3.weights` *(See note)*
	* `git-lfs` to push yolo files.

Note: Due to filesize limitation you may need to download this from the author website `https://pjreddie.com/media/files/yolov3.weights` and save it under `data/yolov3/` directory) or run this wget command and save it to data directory, you are at that project work directory.

`wget https://pjreddie.com/media/files/yolov3.weights -P data/yolov3/`

**Note:** You can run the python library installation by using `pip` by running this on your project root directory `pip3 install -r requirements.txt`

If you want to add new library you need to --
1. Create a new branch and want to commit please run `pip3 freeze > requirements.txt` and create your own branch (see **Contribution guidelines > Branch prefix** for more details) and create pull-request merging towards `staging` branch.


### How do I get set up? ###

* Install your preferred IDE, i recommend `pyCharm`
* I also recommend the use of python virtual environment `venv`. See [Creation of virtual environments](https://docs.python.org/3/library/venv.html).
* See `requirements.txt` python library dependencies
