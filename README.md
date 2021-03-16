# tom-cameratrap

Script for submitting megadetector to the a HPC

## run
```bash
python mega_model.py [PATH]
```
## join output
```bash
python mega_model.py [PATH] --join-json
```
## run folder as a single job
```bash
python mega_model.py [PATH] --single-job
```

## remove path from json files 
```bash
sed 's+Camera_trap_data/Koombooloomba/++g' Camera_trap_data/Koombooloomba/Koombooloomba.json > new.json
```
```bash
# match Koombooloomba_1 to Koombooloomba_6
sed 's+Camera_trap_data/Koombooloomba_[1-6]/++g' Camera_trap_data/Koombooloomba/Koombooloomba.json > new.json
```
## setup

You need a conda env `cameratraps-detector` (see megadetector).
