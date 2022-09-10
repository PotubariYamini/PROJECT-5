Lymphography-NEUTRAL NETWORKS

1. About the dataset:
* This is one of three domains provided by the Oncology Institute that has repeatedly appeared in the machine learning literature. (See also breast-cancer and primary-tumor.)
* Target Variable
class: normal find, metastases, malign lymph, fibrosis

2. Description of Variables:
* lymphatics: normal, arched, deformed, displaced
* block of affere: no, yes
* bl. of lymph. c: no, yes
* bl. of lymph. s: no, yes
* by pass: no, yes
* extravasates: no, yes
* regeneration of: no, yes
* early uptake in: no, yes
* lym.nodes dimin: 0-3
* lym.nodes enlar: 1-4
* changes in lym.: bean, oval, round
* defect in node: no, lacunar, lac. marginal, lac. central
* changes in node: no, lacunar, lac. margin, lac. central
* changes in stru: no, grainy, drop-like, coarse, diluted, reticular, stripped, faint,
* special forms: no, chalices, vesicles
* dislocation of: no, yes
* exclusion of no: no, yes
* no. of nodes in: 0-9, 10-19, 20-29, 30-39, 40-49, 50-59, 60-69, >=70

3. Requirements:
* python
* jupyter notebook
* numpy
* pandas
* tensorflow keras
* imblearn
* searborn , matplotlib
* sklearn libarires

4. EDA of dataset:
* Load the dataset:
by using pandas library
* Majority of the classes 2 (metastases) and 3 (malign lymph) dominate the dataset. While the classes 4 (fibrosis) and 1 (normal find) are really under-represented.
Because of this, we will create and compare models trained using the upsampled data and the regular (not upsampled) data.
* checking the missing values and then doing explorative analysis.

5. Prepare the Data for Modelling:
* rain-Test Split:
As usual, we should separate the target variable from the predictors then split the data into train and test sets.
* Upsample / Oversample:
We've seen above that the dataset is imbalanced. As a workaround, we will upsample/oversample minority classes so that its count is same as the major classes
To do this, we should first merge the x_train and y_train. Shown below is the value counts of target variable before upsampling.


6. Build the model:
* K-Nearest Neighbors:
















