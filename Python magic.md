## numpy stack
Append all elements into an array A

This and  can turn empty into a stack
```python
result = np.stack(A, axis=-1) #or other axis.
```
    
## matplotlib outfit change
```python
import matplotlib.pyplot as plt
import seaborn as sns

color_list = [CB91_Blue, CB91_Pink, CB91_Green, CB91_Amber,
                CB91_Purple, CB91_Violet]
plt.rcParams['axes.prop_cycle'] = plt.cycler(color=color_list)

sns.set(font='Franklin Gothic Book',
        rc={
    'axes.axisbelow': False,
    'axes.edgecolor': 'lightgrey',
    'axes.facecolor': 'None',
    'axes.grid': False,
    'axes.labelcolor': 'dimgrey',
    'axes.spines.right': False,
    'axes.spines.top': False,
    'figure.facecolor': 'white',
    'lines.solid_capstyle': 'round',
    'patch.edgecolor': 'w',
    'patch.force_edgecolor': True,
    'text.color': 'dimgrey',
    'xtick.bottom': False,
    'xtick.color': 'dimgrey',
    'xtick.direction': 'out',
    'xtick.top': False,
    'ytick.color': 'dimgrey',
    'ytick.direction': 'out',
    'ytick.left': False,
    'ytick.right': False})
sns.set_context("notebook", rc={"font.size":16,
                                "axes.titlesize":20,
                                "axes.labelsize":18})

plt.hist(total_err, num_bins,color=CB91_Blue)
```
    
## debug
```python
import pdb
pdb.set_trace()

gdb python
run xxxx.py
```
    
## ptpython
```python
# 高级python
pip install ptpython
```

## Test a website locally
```bash
python3 -m http.server -Web locally
```

## Install pytorch with specific version
```bash
conda install pytorch==1.0.1 torchvision==0.2.2 -c pytorch
```
```
