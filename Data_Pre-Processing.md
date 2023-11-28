## How to Pre_process the data???
#### Datas are two types
1. Structured Data set (tables,csv,excel) => Machine Learning 
2. Unstructured Data set  (Audio,Vedio,image )=> Deep learning

### The following Techniques are there for pre-processing the data to handle missiging value. garbage value 
- Step1:
   - Handling missing value        (applicable for both categorical and numerical data type)
- Step_2:
  - Handling Outlier       (applicable for numerical data type)
-  Step 3:
  - Handling Encoding part       (applicable for categorical data type)
    - Step_2.1: Label Encoder
    - Step_2.2 : One Hot Encoder
    - Step2.3 : Dummy Variable
- Step_4:
  - Feature Scaling           (applicable for numerical data type)
    - Step_4.1 : Normalisation
    - Step_4.2 : Standardisation
- Step_5 :
   - Handling Imbalance Dataset (this is applicable for Classification Problem)
 
### Step_1: Handling missing value
  - Rule_1 :
    - if 25% or more data missed, ignore/drop that variable
  - Ruel_2:
    - if less than 25% data is missed,
    - Step_1: Check the data type of that variable (number or character(object))
    - Step_2: if the variable is Character / object => do MODE approach
    - Step_3: if the vauiable is number
       - The approach is to first check outliers
       - if outliers found, use MEDIAN
       - if no outliers , then use MEAN


#### Outlier:
- Calculation of Quartile:
   - Suppose a dataset contain n number of data then 
   - quartile_1 = (n+1)/4     => 25th percentile
   - quartile_2 = (n+1)/2     => 50th percentile
   - quartile_3 = 3(n+1)/4     => 75th percentile
   - quartile_4 = (n+1)        => 100th percentile
- InterQuartileRange (IQR) = quartile_3 - quartile_1
- Positive Outlier = quartile_3 + 1.5 * IQR        => 1.5 is 15% threshold value. It depends on the client to change to 10 or 20 percent
- Negative Outlier = quartile_1 - 1.5 * IQR

### Step_2: Handling Outliers:
- If outliers found in Dataset
- Transformation approach is:
   - General Approach (quartile_3 + 1.5 * IQR or quartile_1 - 1.5 * IQR)
   - Square root
        - By transforming the data into square root values, the removal of data is omitted
   - Cube root
        - By transforming the data into cube root values, the removal of data is omitted (more data is saved from removal process)
   - Log Transformation
        - By transforming the data into log values, the removal of data is almost omitted (because all  data values transformed to minimum scale values) 
 
- Regularisation Approach
  - Lasso/Ridge / ElasticNet
  - Hetroscadicity
 
### Step_3: Handling Encoding part 
- Label Encoder:
     - Categories variables are converted into numerical values by assigning a sample number to that variable (similar to sorting an alphabetical list)
- One Hot Encoder:
     - converting label encode to bit of 0 and 1 values


#### Important Module/Library to use in Data_Preprocessing
- Numpy
- Pandas
- Matplotlib.pyplot
- Seaborn
