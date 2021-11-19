# Vehicle-Counter-VCNET
method proposes a low-cost solution for vehicle counting in highway images. This approach, which considers the problem as a deep learning-based classification problem, classifies the signature differences created by road and vehicle sections

# Install
Use the package manager pip to install requirements
```bash
pip install -r requirements.txt
```

# Inferance

## Roi Selection
run below command, follow instructions and save roi's as a json file
```bash
python3 roiSelector.py --video M30-HD.avi --name M30-HD
```
output json will generated named as M30-HD.json

## Video inferance
run below command for inferance

```bash
python3 main.py --video M30-HD.avi --json M30-HD.json --model model/vehicle_counter.h5
``
