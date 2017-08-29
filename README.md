# scipy-scan-show_exp-extract_data
Using REST interface to Scan for Minicubes, List Experiment in a selected minicube and extra data from an experiment

We used Python 2.7 installed via Anaconda install. 
This project is made in Jupyter Notebook but uses two external python files.

External files
1. minicube.py
2. pypcr_v31.py


Following imports are used :

from six.moves import input
from zeroconf import ServiceBrowser, Zeroconf
import time
import requests
import socket
import csv
import sys
import argparse

In Jupyter Notebook correct paths to the external files must be given. 

An output path to the CSV files extracted from the minicube must be given otherwise it will store the CSV files in the current directory which often will be your Jupyter Notebook home dir. 

#KNOWN BUGS
Sometimes the cell in the jupyter notebook that scans the network for avaialble minicubes fails on the first scan. 
Fix: Just rerun the cell a second time

