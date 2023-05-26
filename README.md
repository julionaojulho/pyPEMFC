# pyPEMFC
Python 3 module for proton-exchange membrane fuel cells

```
import pyPEMFC as FC

conditions = FC.sample_loader(0) # dictionary of FC sample conditions
PEMFC = FC.set_conditions(conditions)
PEMFC.initial_temperature = 300 # K
PEMFC.cathodePressure = 5e5     # Pa
PEMFC.anodePressure = 3e5       # Pa
PEMFC.anodeFuel = 'H2'
PEFMC.cathodeGas = 'O2'
PEMFC.solver(method='FD')
```
