# Module_14_machine_learning_trading_bot
GWU FinTech Bootcamp Module 14 Challenge 

**A Jupyter notebook that uses machine learning trading bots for automated trading. Several different models were used and tuned to produce the best results.**

Here's the first model with the shorter training period. After tuning the model in model2 with a training period that is twice as long, it is clear that the longer training period produces better results.

![Screenshot](https://github.com/jimhitchcock/Module_14_machine_learning_trading_bot/blob/main/Resources/Model_1.png)

Here's the second model with the longer training period. This model produced a higher accuracy score and cumulative returns than the shorter period later in the dataset.  Early in the dataset, the model's predictions where below the actual results, this changed later in the dataset.

![Screenshot](https://github.com/jimhitchcock/Module_14_machine_learning_trading_bot/blob/main/Resources/Model_2.png)

Here's the third model (Logistic Regresssion) which shows that it was pretty accurate earlier in the dataset but the accuracy plummets toward the end of the dataset.

![Screenshot](https://github.com/jimhitchcock/Module_14_machine_learning_trading_bot/tree/main/Resources/Model_3.png)

---

## Technologies

[Pandas](https://pandas.pydata.org/)

[hvplot.pandas](https://hvplot.holoviz.org/user_guide/Plotting.html)

[Numpy](https://numpy.org/)

[sklearn](https://scikit-learn.org/stable/)

---

## Installation Guide

```python
import pandas as pd
import numpy as np
from pathlib import Path
import hvplot.pandas
import matplotlib.pyplot as plt
from sklearn import svm
from sklearn.preprocessing import StandardScaler
from pandas.tseries.offsets import DateOffset
from sklearn.metrics import classification_report
```
---

## Conclusions

**We have determined that Model_2, the model with the longer training period and the SVC classifer model, produced the better accuracy results, especially later in the dataset than the Logistic Regression model or the first SVC classifer model with the shorter training period.  Although continued tuning and modifications are always recommended, model_2 produced the best resutls over the testing period.

---

## Contributors

Parts of this application were written by Jim Hitchcock, starter code provided by GWU FinTech Bootcamp.

---

## License

MIT License.