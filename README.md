# Epileptic-Seizure-Detection
Epileptic Seizure Detection using Deep Learning and Adaptive Filters
##Requirements: -

###system requirements:

-Python 3.6 or higher
-pip3
-Jupyter Notebook (Sublime Text or any other will work as well)

###installation:

####Python3
 Follow the link "https://realpython.com/installing-python/". From there download and install python3 as per your OS(windows, Mac or Linux)

####Pip
1.Follow the link "https://www.liquidweb.com/kb/install-pip-windows/" for installation
2.Upgrade pip for python3
run the command in cmd "python -m pip install -U pip" and make sure pip is compatible with python3

####Jupyter Notebook
1.Follow the link "https://jupyter.readthedocs.io/en/latest/install.html" for installation
Or alternatively if pip3 and python3 are compatible and running use the following command on cmd "pip3 install jupyter"

###Dataset
The dataset used in this project is the publically available data prepared by CHB-MIT and available for use. This can be downloaded from this link "https://www.physionet.org/pn6/chbmit/"

###Libraries
The following libaries are required for running the codes

-numpy 
-scipy
-matplotlib
-pyedflib
-pandas
-padasip
-keras
-math

these are stored in libraries.txt 

Install all these libraries individually or use this command to install "pip3 install -r libraries.txt"

##Running the codes: -

-Open the Jupyter Notebook in the folder 'All_seizures' where all the key files have been stored

-Run the nlms_on_CHB.py for getting the adaptive filter
-Run the channel_selection.py for selecting the channels. Results will be stored in selected_channels.txt

####Set the paths and parameters:
Open load.txt in a text reader and add the path to the following-
1.pathDataset:'insert path' (add the path of dataset here like this ....pn6/chbmit/)
2.FirstPartPathOutput: 'insert path' (add the path where the result will be saved, which will be used later)

Open cnn_final.py and add the following paths-
1.PathSpectrogramFolder='insert path' (path where the results are saved. same as FirstPartPathOutput)
2.OutputPath='insert path' (path where to save results)
3.OutputPathModels='insert path' (path for results produced)
Open dcgan_final.py and follow the same steps as done for cnn_final.py

-Run the make_Stft.py file
-Run the cnn_final.py file
-Run the dcgan_final.py file

