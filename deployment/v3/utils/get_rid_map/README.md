# RID-UIN Map Utility

## Overview
Utlity that returns UINs corresponding to RIDs.  Input is a list of RIDs in file. Output is RID-UID map generated in CSV format.

**STRICT WARNING:**  This script is to be used for development purposes only.  

## Prerequisites
1. Python3.9
1. Set up python3.9 virtual env
    ```sh
    mkdir ~/.venv
    python3.9 -m venv ~/.venv/myenv
    ```
1. Switch to virtual env 
    ```
    source ~/.venv/myenv/bin/activate
    ```
1. Install required modules
    ```sh
    pip install -r requirements.txt
    ```

## Run

```
python get_rid_map.py <rid file> <out csv>
```

## RID file
Example:

```
10002100870000120211223074113
10002100880000120211129132529
10002100871300120211129132529
```