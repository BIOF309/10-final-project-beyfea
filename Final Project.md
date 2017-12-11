
<font size = "6px"><center>Ligand Preferences of Innate Immune Receptor RIG-I</font></center>

<font size = "4px"><center>Chen Wang</font></center>
<font size = "4px"><center>Rutgers, The State University of New Jersey</font></center>
<font size = "4px"><center>National Institute of Allergy and Infectious Diseases/National Institutes of Health</font></center>

## Biochemical Studies of RIG-I in the Presence of 5’OH, 5’ppp, Cap-0 24mer Hairpin (HP) RNAs

<table>
<tr>
    <th>    </th>
    <th>WT RIG-I      </th>
    </tr>
    <tr>
        <td>RNA ligand</td>
        <td>$K_{d,app}(nM)$</td>
        <td>$k_{atpase}$ ($s^{-1}$)</td>
    </tr>
    <tr>
        <td>5'OH HP RNA</td>
        <td>38.5 $\pm$ 4</td>
        <td>49 $\pm$ 1</td>
    </tr>
    <tr>
        <td>5'ppp HP RNA</td>
        <td>1.8 $\pm$ 0.9</td>
        <td>33 $\pm$ 0.9</td>
    </tr>
    <tr>
        <td>Cap-0 HP RNA</td>
        <td>1.7 $\pm$ 0.5</td>
        <td>25 $\pm$ 0.4</td>

## Crystal Structures of RIG-I Helicase-RD with 5’OH, 5’ppp, Cap-0 24mer HP RNAs

![title](Picture1.png)

## Interaction of 2’-OH on First Nucleotide with Histidine 830 (H830)

![title](Picture2.png)

<table>
<tr>
    <th>    </th>
    <th>WT</th>
    <th>RIG-I</th>
    <th>H830A</th>
    <th>RIG-I</th>
    </tr>
    <tr>
        <td>RNA ligand</td>
        <td>$K_{d,app}(nM)$</td>
        <td>$k_{atpase}$ ($s^{-1}$)</td>
        <td>$K_{d,app}(nM)$</td>
        <td>$k_{atpase}$ ($s^{-1}$)</td>
    </tr>
    <tr>
        <td>5'ppp HP RNA</td>
        <td>1.8 $\pm$ 0.9</td>
        <td>33 $\pm$ 0.9</td>
        <td>1.6 $\pm$ 1.9</td>
        <td>34 $\pm$ 1</td>
    </tr>
    <tr>
        <td>5'ppp 2'-OMe HP RNA</td>
        <td>40 $\pm$ 5</td>
        <td>12 $\pm$ 0.4</td>
        <td>2.3 $\pm$ 0.7</td>
        <td>32 $\pm$ 0.5</td>
    </tr>
    <tr>
        <td>Cap-0 HP RNA</td>
        <td>1.7 $\pm$ 0.5</td>
        <td>25 $\pm$ 0.4</td>
        <td>1.9 $\pm$ 0.5</td>
        <td>22 $\pm$ 0.4</td>
    </tr>
    <tr>
        <td>Cap-1 HP RNA</td>
        <td>425 $\pm$ 50</td>
        <td>15 $\pm$ 0.7</td>
        <td>9.5 $\pm$ 2</td>
        <td>24 $\pm$ 0.3</td>

## Cell-based Reporter Signaling Assays


```python
#IFN signal data showed in bar chart with matplotlib
import numpy as np
import matplotlib.pyplot as plt
 
size = 5
x = np.arange(size)
a = [3.9, 8.0, 8.5, 2.1, 2.05]
b = [3.8, 8.2, 11, 6.1, 2.15]
aerror = [0.2, 0.2, 0.2, 0.1, 0.15]
berror = [0.25, 1, 1, 0.8, 0.2]
 
total_width, n = 0.8, 3
width = total_width / n
x = x - (total_width - width) / 2
 
plt.bar(x, a, yerr=aerror, width=width, label='WT RIG-I')
plt.bar(x + width, b, yerr=berror, width=width, label='H830A RIG-I')
plt.legend()
plt.show()
```


![png](Final%20Project_files/Final%20Project_9_0.png)


## Summary

### RIG-I recognizes Cap-0 dsRNAs as efficiently as 5′ppp dsRNAs.
### RIG-I accommodates the m7G cap without perturbation of the ppp moiety interactions.
### 2’-O-methylation on the first nucleotide of RNA 5’ end is critical for RIG-I discrimination.
### H830 residue is the primary sensor of 2′-O-methylation in Cap-1 dsRNA. 
