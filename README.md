june-3-2021

Operating system tested with :
windows 

other operating system will work  but you have to collect respective compiled  version for node2vec.
in this repo for windows we have used the version located in "........\\GEM\\Snap-6.0-Win32\\node2vec.exe"

you can download respective os version here :
https://snap.stanford.edu/snap/download.html

also i have put backup  here: 
https://ahsan-nmsu.s3-us-west-1.amazonaws.com/Snap-6.0-Win32.zip

https://ahsan-nmsu.s3-us-west-1.amazonaws.com/Snap-6.0-macOS14.10.tgz

https://ahsan-nmsu.s3-us-west-1.amazonaws.com/Snap-6.0-Ubuntu18.04.tgz


requirments:

Python 3.6.8 (to check defult python version run cmd: python --version )
if you have a deiffrent pythin version than make sure to activate proper version as deafult python
or
emplictly you can point to version 3.6.8's path on your cmds

python modules:
https://stackoverflow.com/questions/33751214/single-command-in-python-to-install-relevant-modules-from-a-package-json-like-fi
(module name== version )

bleach==1.5.0
cached-property==1.5.2
cycler==0.10.0
decorator==4.4.2
h5py==3.1.0
html5lib==0.9999999
importlib-metadata==3.4.0
Keras==2.0.2
kiwisolver==1.3.1
Markdown==3.3.3
matplotlib==2.2.3
networkx==1.11
numpy==1.19.5
Pillow==8.1.0
protobuf==3.15.1
pyparsing==2.4.7
python-dateutil==2.8.1
pytz==2021.1
PyYAML==5.4.1
scikit-learn==0.19.0
scipy==1.5.4
six==1.15.0
snap-stanford==6.0.0
tensorflow==1.3.0
tensorflow-tensorboard==0.1.8
Theano==1.0.4
typing-extensions==3.7.4.3
Werkzeug==1.0.1
zipp==3.4.0

To install all these modules at once you can run this cmd insode root folder of the cloned repo:
pip install -r requirements.txt

this cmd will install all the required version written in requirements.txt(this file exist in the root folder of the repo)





update node2vec excutable for your OS :

open node2vec.py and find :
args = ["C:\\Users\\......\\.......\\GEM\\Snap-6.0-Win32\\node2vec.exe"]

update the path based on location whre you have kept the  node2vec excutable. for windows i ahve put it  in  the Gem folder :
......\GEM\Snap-6.0-Win32\node2vec.exe



once alldone than  run these cmds in root folder to test if everything ok or not:

python test_karate.py -node2vec 0 
python test_karate.py -node2vec 1


need to fix:
python test_sbm.py -node2vec 0
python test_sbm.py -node2vec 1
