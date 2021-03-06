# Vehicle-Counter-VCNET
method proposes a low-cost solution for vehicle counting in highway images. This approach, which considers the problem as a deep learning-based classification problem, classifies the signature differences created by road and vehicle sections

M-30HD highway performance
[Watch the video](https://www.youtube.com/watch?v=sZ_sz6R3ET0)

Izmit highway performance
[Watch the video](https://www.youtube.com/watch?v=mj69vIJ-eDU)


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
![Roi selection](https://user-images.githubusercontent.com/37477289/142638864-771230d3-91e6-403c-a89f-53fa1f81d6e8.png)

output json will generated named as M30-HD.json

## Video inferance
run below command for inferance

```bash
python3 main.py --video M30-HD.avi --json M30-HD.json --model model/vehicle_counter.h5
```
![VCNET](https://user-images.githubusercontent.com/37477289/142639212-4cdbb0d2-f134-45ce-8a0f-4873dc5c5cf3.png)
