
```
conda create -n dni python=3.10
conda activate mambaD
cd Tuning_free_mambaD
pip install -r requirements.txt
```

## DDIM inversion

Preprocess you video by running using the following command:
```
python ddim_inversion.py
```
## Editing
```
python dni.py
```

## Environment for tuning based DNI
```
conda create -n dni_tuning python=3.10
conda activate mambaD_tuning
cd Tuning_mambaD
pip install -r requirements.txt
```

## model tuning

Preprocess you video by running using the following command:
```
python dni_tuning.py
```
## Editing
```
python dni.py
```

