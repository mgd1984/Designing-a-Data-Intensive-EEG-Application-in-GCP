# Designing a Data Intensive EEG Application in GCP

Capstone project for 3252 - Big Data Tools of the Data Science Fundamental program at the University of Toronto SCS - Fall 2017. The report was written to demonstrate how popular big data tools (i.e. Spark, Hadoop, MQTT, etc.) could be used to create a data intensive EEG (brain wave) application using the Google Cloud Platform (GCP).

See attached [PDF](https://github.com/mgd1984/Designing-a-Data-Intensive-EEG-Application-in-GCP/blob/master/3252%20Final%20Project%20Report%20%E2%80%93%20Designing%20a%20Data%20Intensive%20EEG%20Application.pdf) for full report describing background, methodology, and results. 

### Application Architecture 

### Using MusePython to Send EEG Data to GCP  
The [MusePython.py](https://github.com/mgd1984/Designing-a-Data-Intensive-EEG-Application-in-GCP/blob/master/MusePython.py) library provides a way to send Muse EEG data to the cloud over UDP.

There is also [Muse-LSL](https://github.com/alexandrebarachant/muse-lsl) which provides another set of scripts that use the newer 2016 Muse headset. For my purposes, I have an older Muse headset, so I went with the MusePython.py library as referenced on the InteraXon [developer page](http://developer.choosemuse.com/research-tools-example/grabbing-data-from-museio-a-few-simple-examples-of-muse-osc-servers#python) 

### A Note About LSL - Lab Streaming Layer 
[LSL](https://github.com/sccn/labstreaminglayer) (Lab Streaming Layer) is a suite of software utilities for the unified collection and measurement of time series in research experiments that handles both the networking, time-synchronization, (near-) real-time access as well as optionally the centralized collection, viewing and disk recording of the data.' [[Source]](https://github.com/sccn/labstreaminglayer). The software was developed at the Swartz Centre for Computational Neuroscience at the University of San Diego [[link]](https://sccn.ucsd.edu/people/). 

### Use EEGrunt to Analyze EEG Data in the Cloud  
[EEGrunt](https://github.com/curiositry/EEGrunt) is a collection of EEG analysis tools, written in Python. It is compatible with the original Muse headset from 2014 and can be used to run analysis on streaming EEG data. 

###


