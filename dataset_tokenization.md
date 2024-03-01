```python
#install neccessary library
!pip install nltk pandas

```

    Collecting nltk
      Downloading nltk-3.8.1-py3-none-any.whl.metadata (2.8 kB)
    Collecting pandas
      Downloading pandas-2.2.1-cp312-cp312-win_amd64.whl.metadata (19 kB)
    Requirement already satisfied: click in c:\users\administrator\appdata\local\programs\python\python312\lib\site-packages (from nltk) (8.1.7)
    Collecting joblib (from nltk)
      Downloading joblib-1.3.2-py3-none-any.whl.metadata (5.4 kB)
    Collecting regex>=2021.8.3 (from nltk)
      Downloading regex-2023.12.25-cp312-cp312-win_amd64.whl.metadata (41 kB)
         ---------------------------------------- 0.0/42.0 kB ? eta -:--:--
         ---------------------------------------- 42.0/42.0 kB 1.0 MB/s eta 0:00:00
    Collecting tqdm (from nltk)
      Downloading tqdm-4.66.2-py3-none-any.whl.metadata (57 kB)
         ---------------------------------------- 0.0/57.6 kB ? eta -:--:--
         ---------------------------------------- 57.6/57.6 kB 3.0 MB/s eta 0:00:00
    Collecting numpy<2,>=1.26.0 (from pandas)
      Downloading numpy-1.26.4-cp312-cp312-win_amd64.whl.metadata (61 kB)
         ---------------------------------------- 0.0/61.0 kB ? eta -:--:--
         ---------------------------------------- 61.0/61.0 kB 3.2 MB/s eta 0:00:00
    Requirement already satisfied: python-dateutil>=2.8.2 in c:\users\administrator\appdata\local\programs\python\python312\lib\site-packages (from pandas) (2.8.2)
    Collecting pytz>=2020.1 (from pandas)
      Downloading pytz-2024.1-py2.py3-none-any.whl.metadata (22 kB)
    Requirement already satisfied: tzdata>=2022.7 in c:\users\administrator\appdata\local\programs\python\python312\lib\site-packages (from pandas) (2023.3)
    Requirement already satisfied: six>=1.5 in c:\users\administrator\appdata\local\programs\python\python312\lib\site-packages (from python-dateutil>=2.8.2->pandas) (1.16.0)
    Requirement already satisfied: colorama in c:\users\administrator\appdata\local\programs\python\python312\lib\site-packages (from click->nltk) (0.4.6)
    Downloading nltk-3.8.1-py3-none-any.whl (1.5 MB)
       ---------------------------------------- 0.0/1.5 MB ? eta -:--:--
       ------- -------------------------------- 0.3/1.5 MB 8.9 MB/s eta 0:00:01
       --------------- ------------------------ 0.6/1.5 MB 7.4 MB/s eta 0:00:01
       --------------------------- ------------ 1.0/1.5 MB 7.3 MB/s eta 0:00:01
       ------------------------------------- -- 1.4/1.5 MB 8.3 MB/s eta 0:00:01
       ---------------------------------------- 1.5/1.5 MB 8.0 MB/s eta 0:00:00
    Downloading pandas-2.2.1-cp312-cp312-win_amd64.whl (11.5 MB)
       ---------------------------------------- 0.0/11.5 MB ? eta -:--:--
        --------------------------------------- 0.2/11.5 MB 7.6 MB/s eta 0:00:02
       - -------------------------------------- 0.6/11.5 MB 7.0 MB/s eta 0:00:02
       --- ------------------------------------ 0.9/11.5 MB 7.2 MB/s eta 0:00:02
       ---- ----------------------------------- 1.2/11.5 MB 7.0 MB/s eta 0:00:02
       ---- ----------------------------------- 1.4/11.5 MB 7.3 MB/s eta 0:00:02
       ------ --------------------------------- 1.7/11.5 MB 6.5 MB/s eta 0:00:02
       ------ --------------------------------- 2.0/11.5 MB 6.3 MB/s eta 0:00:02
       ------- -------------------------------- 2.2/11.5 MB 6.1 MB/s eta 0:00:02
       -------- ------------------------------- 2.4/11.5 MB 6.0 MB/s eta 0:00:02
       --------- ------------------------------ 2.8/11.5 MB 6.1 MB/s eta 0:00:02
       ---------- ----------------------------- 3.1/11.5 MB 6.3 MB/s eta 0:00:02
       ------------ --------------------------- 3.5/11.5 MB 6.3 MB/s eta 0:00:02
       ------------ --------------------------- 3.6/11.5 MB 6.1 MB/s eta 0:00:02
       ------------- -------------------------- 3.9/11.5 MB 6.1 MB/s eta 0:00:02
       -------------- ------------------------- 4.1/11.5 MB 5.8 MB/s eta 0:00:02
       -------------- ------------------------- 4.2/11.5 MB 5.7 MB/s eta 0:00:02
       --------------- ------------------------ 4.4/11.5 MB 5.6 MB/s eta 0:00:02
       ---------------- ----------------------- 4.7/11.5 MB 5.6 MB/s eta 0:00:02
       ----------------- ---------------------- 5.1/11.5 MB 5.7 MB/s eta 0:00:02
       ------------------- -------------------- 5.5/11.5 MB 5.8 MB/s eta 0:00:02
       -------------------- ------------------- 5.8/11.5 MB 5.9 MB/s eta 0:00:01
       --------------------- ------------------ 6.1/11.5 MB 5.9 MB/s eta 0:00:01
       ---------------------- ----------------- 6.5/11.5 MB 6.0 MB/s eta 0:00:01
       ----------------------- ---------------- 6.7/11.5 MB 6.0 MB/s eta 0:00:01
       ------------------------ --------------- 7.0/11.5 MB 6.1 MB/s eta 0:00:01
       ------------------------- -------------- 7.2/11.5 MB 5.9 MB/s eta 0:00:01
       ------------------------- -------------- 7.4/11.5 MB 5.8 MB/s eta 0:00:01
       -------------------------- ------------- 7.6/11.5 MB 5.7 MB/s eta 0:00:01
       --------------------------- ------------ 7.8/11.5 MB 5.7 MB/s eta 0:00:01
       --------------------------- ------------ 8.0/11.5 MB 5.6 MB/s eta 0:00:01
       ---------------------------- ----------- 8.1/11.5 MB 5.5 MB/s eta 0:00:01
       ---------------------------- ----------- 8.3/11.5 MB 5.4 MB/s eta 0:00:01
       ----------------------------- ---------- 8.4/11.5 MB 5.4 MB/s eta 0:00:01
       ----------------------------- ---------- 8.5/11.5 MB 5.3 MB/s eta 0:00:01
       ------------------------------ --------- 8.7/11.5 MB 5.2 MB/s eta 0:00:01
       ------------------------------ --------- 8.8/11.5 MB 5.2 MB/s eta 0:00:01
       ------------------------------- -------- 8.9/11.5 MB 5.1 MB/s eta 0:00:01
       ------------------------------- -------- 9.1/11.5 MB 5.1 MB/s eta 0:00:01
       -------------------------------- ------- 9.2/11.5 MB 5.0 MB/s eta 0:00:01
       -------------------------------- ------- 9.4/11.5 MB 5.0 MB/s eta 0:00:01
       --------------------------------- ------ 9.7/11.5 MB 5.0 MB/s eta 0:00:01
       ---------------------------------- ----- 9.9/11.5 MB 5.0 MB/s eta 0:00:01
       ----------------------------------- ---- 10.1/11.5 MB 5.0 MB/s eta 0:00:01
       ----------------------------------- ---- 10.3/11.5 MB 4.9 MB/s eta 0:00:01
       ------------------------------------ --- 10.6/11.5 MB 4.9 MB/s eta 0:00:01
       ------------------------------------- -- 10.8/11.5 MB 4.9 MB/s eta 0:00:01
       -------------------------------------- - 11.0/11.5 MB 4.9 MB/s eta 0:00:01
       ---------------------------------------  11.4/11.5 MB 4.9 MB/s eta 0:00:01
       ---------------------------------------  11.5/11.5 MB 4.8 MB/s eta 0:00:01
       ---------------------------------------- 11.5/11.5 MB 4.8 MB/s eta 0:00:00
    Downloading numpy-1.26.4-cp312-cp312-win_amd64.whl (15.5 MB)
       ---------------------------------------- 0.0/15.5 MB ? eta -:--:--
        --------------------------------------- 0.2/15.5 MB 12.2 MB/s eta 0:00:02
       - -------------------------------------- 0.5/15.5 MB 6.0 MB/s eta 0:00:03
       - -------------------------------------- 0.7/15.5 MB 5.2 MB/s eta 0:00:03
       -- ------------------------------------- 0.9/15.5 MB 5.2 MB/s eta 0:00:03
       --- ------------------------------------ 1.2/15.5 MB 5.5 MB/s eta 0:00:03
       --- ------------------------------------ 1.4/15.5 MB 5.6 MB/s eta 0:00:03
       ---- ----------------------------------- 1.7/15.5 MB 5.6 MB/s eta 0:00:03
       ---- ----------------------------------- 1.9/15.5 MB 6.0 MB/s eta 0:00:03
       ---- ----------------------------------- 1.9/15.5 MB 6.0 MB/s eta 0:00:03
       ---- ----------------------------------- 1.9/15.5 MB 6.0 MB/s eta 0:00:03
       ----- ---------------------------------- 2.0/15.5 MB 4.3 MB/s eta 0:00:04
       ----- ---------------------------------- 2.3/15.5 MB 4.3 MB/s eta 0:00:04
       ------ --------------------------------- 2.4/15.5 MB 4.4 MB/s eta 0:00:03
       ------ --------------------------------- 2.4/15.5 MB 4.4 MB/s eta 0:00:03
       ------ --------------------------------- 2.4/15.5 MB 4.4 MB/s eta 0:00:03
       ------ --------------------------------- 2.4/15.5 MB 4.4 MB/s eta 0:00:03
       ------ --------------------------------- 2.4/15.5 MB 4.4 MB/s eta 0:00:03
       ------ --------------------------------- 2.4/15.5 MB 3.1 MB/s eta 0:00:05
       ------ --------------------------------- 2.5/15.5 MB 3.0 MB/s eta 0:00:05
       ------ --------------------------------- 2.7/15.5 MB 3.1 MB/s eta 0:00:05
       ------- -------------------------------- 3.0/15.5 MB 3.2 MB/s eta 0:00:04
       -------- ------------------------------- 3.1/15.5 MB 3.2 MB/s eta 0:00:04
       -------- ------------------------------- 3.2/15.5 MB 3.2 MB/s eta 0:00:04
       -------- ------------------------------- 3.3/15.5 MB 3.2 MB/s eta 0:00:04
       -------- ------------------------------- 3.4/15.5 MB 3.1 MB/s eta 0:00:04
       --------- ------------------------------ 3.6/15.5 MB 3.2 MB/s eta 0:00:04
       --------- ------------------------------ 3.7/15.5 MB 3.1 MB/s eta 0:00:04
       --------- ------------------------------ 3.8/15.5 MB 3.1 MB/s eta 0:00:04
       ---------- ----------------------------- 3.9/15.5 MB 3.0 MB/s eta 0:00:04
       ---------- ----------------------------- 4.0/15.5 MB 3.0 MB/s eta 0:00:04
       ---------- ----------------------------- 4.1/15.5 MB 2.9 MB/s eta 0:00:04
       ---------- ----------------------------- 4.2/15.5 MB 2.9 MB/s eta 0:00:04
       ----------- ---------------------------- 4.4/15.5 MB 2.9 MB/s eta 0:00:04
       ----------- ---------------------------- 4.4/15.5 MB 2.9 MB/s eta 0:00:04
       ----------- ---------------------------- 4.6/15.5 MB 2.9 MB/s eta 0:00:04
       ----------- ---------------------------- 4.6/15.5 MB 2.9 MB/s eta 0:00:04
       ------------ --------------------------- 4.8/15.5 MB 2.9 MB/s eta 0:00:04
       ------------ --------------------------- 4.9/15.5 MB 2.9 MB/s eta 0:00:04
       ------------ --------------------------- 5.0/15.5 MB 2.9 MB/s eta 0:00:04
       ------------- -------------------------- 5.1/15.5 MB 2.8 MB/s eta 0:00:04
       ------------- -------------------------- 5.1/15.5 MB 2.8 MB/s eta 0:00:04
       ------------- -------------------------- 5.2/15.5 MB 2.8 MB/s eta 0:00:04
       ------------- -------------------------- 5.3/15.5 MB 2.8 MB/s eta 0:00:04
       -------------- ------------------------- 5.4/15.5 MB 2.8 MB/s eta 0:00:04
       -------------- ------------------------- 5.6/15.5 MB 2.8 MB/s eta 0:00:04
       -------------- ------------------------- 5.6/15.5 MB 2.8 MB/s eta 0:00:04
       -------------- ------------------------- 5.7/15.5 MB 2.7 MB/s eta 0:00:04
       --------------- ------------------------ 5.9/15.5 MB 2.7 MB/s eta 0:00:04
       --------------- ------------------------ 5.9/15.5 MB 2.7 MB/s eta 0:00:04
       --------------- ------------------------ 6.1/15.5 MB 2.7 MB/s eta 0:00:04
       ---------------- ----------------------- 6.3/15.5 MB 2.7 MB/s eta 0:00:04
       ---------------- ----------------------- 6.3/15.5 MB 2.7 MB/s eta 0:00:04
       ---------------- ----------------------- 6.6/15.5 MB 2.7 MB/s eta 0:00:04
       ----------------- ---------------------- 6.7/15.5 MB 2.7 MB/s eta 0:00:04
       ----------------- ---------------------- 6.8/15.5 MB 2.7 MB/s eta 0:00:04
       ----------------- ---------------------- 6.9/15.5 MB 2.7 MB/s eta 0:00:04
       ------------------ --------------------- 7.0/15.5 MB 2.7 MB/s eta 0:00:04
       ------------------ --------------------- 7.1/15.5 MB 2.7 MB/s eta 0:00:04
       ------------------ --------------------- 7.2/15.5 MB 2.7 MB/s eta 0:00:04
       ------------------ --------------------- 7.3/15.5 MB 2.7 MB/s eta 0:00:04
       ------------------- -------------------- 7.4/15.5 MB 2.7 MB/s eta 0:00:04
       ------------------- -------------------- 7.5/15.5 MB 2.7 MB/s eta 0:00:04
       ------------------- -------------------- 7.6/15.5 MB 2.7 MB/s eta 0:00:03
       ------------------- -------------------- 7.6/15.5 MB 2.7 MB/s eta 0:00:03
       ------------------- -------------------- 7.8/15.5 MB 2.6 MB/s eta 0:00:03
       -------------------- ------------------- 7.9/15.5 MB 2.6 MB/s eta 0:00:03
       -------------------- ------------------- 8.0/15.5 MB 2.6 MB/s eta 0:00:03
       -------------------- ------------------- 8.0/15.5 MB 2.6 MB/s eta 0:00:03
       -------------------- ------------------- 8.1/15.5 MB 2.6 MB/s eta 0:00:03
       --------------------- ------------------ 8.2/15.5 MB 2.6 MB/s eta 0:00:03
       --------------------- ------------------ 8.3/15.5 MB 2.6 MB/s eta 0:00:03
       --------------------- ------------------ 8.4/15.5 MB 2.6 MB/s eta 0:00:03
       --------------------- ------------------ 8.5/15.5 MB 2.6 MB/s eta 0:00:03
       ---------------------- ----------------- 8.6/15.5 MB 2.6 MB/s eta 0:00:03
       ---------------------- ----------------- 8.7/15.5 MB 2.5 MB/s eta 0:00:03
       ---------------------- ----------------- 8.8/15.5 MB 2.5 MB/s eta 0:00:03
       ---------------------- ----------------- 8.9/15.5 MB 2.5 MB/s eta 0:00:03
       ----------------------- ---------------- 9.0/15.5 MB 2.5 MB/s eta 0:00:03
       ----------------------- ---------------- 9.1/15.5 MB 2.5 MB/s eta 0:00:03
       ----------------------- ---------------- 9.2/15.5 MB 2.5 MB/s eta 0:00:03
       ----------------------- ---------------- 9.3/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------ --------------- 9.4/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------ --------------- 9.5/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------ --------------- 9.7/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------- -------------- 9.8/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------- -------------- 9.8/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------- -------------- 9.9/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------- -------------- 9.9/15.5 MB 2.5 MB/s eta 0:00:03
       ------------------------- -------------- 10.1/15.5 MB 2.5 MB/s eta 0:00:03
       -------------------------- ------------- 10.1/15.5 MB 2.5 MB/s eta 0:00:03
       -------------------------- ------------- 10.3/15.5 MB 2.5 MB/s eta 0:00:03
       -------------------------- ------------- 10.4/15.5 MB 2.4 MB/s eta 0:00:03
       -------------------------- ------------- 10.4/15.5 MB 2.4 MB/s eta 0:00:03
       --------------------------- ------------ 10.5/15.5 MB 2.4 MB/s eta 0:00:03
       --------------------------- ------------ 10.5/15.5 MB 2.4 MB/s eta 0:00:03
       --------------------------- ------------ 10.7/15.5 MB 2.4 MB/s eta 0:00:03
       --------------------------- ------------ 10.8/15.5 MB 2.4 MB/s eta 0:00:02
       ---------------------------- ----------- 11.0/15.5 MB 2.4 MB/s eta 0:00:02
       ---------------------------- ----------- 11.2/15.5 MB 2.3 MB/s eta 0:00:02
       ----------------------------- ---------- 11.4/15.5 MB 2.3 MB/s eta 0:00:02
       ----------------------------- ---------- 11.6/15.5 MB 2.3 MB/s eta 0:00:02
       ------------------------------ --------- 11.8/15.5 MB 2.3 MB/s eta 0:00:02
       ------------------------------- -------- 12.1/15.5 MB 2.4 MB/s eta 0:00:02
       -------------------------------- ------- 12.4/15.5 MB 2.4 MB/s eta 0:00:02
       -------------------------------- ------- 12.6/15.5 MB 2.5 MB/s eta 0:00:02
       --------------------------------- ------ 12.9/15.5 MB 2.6 MB/s eta 0:00:02
       ---------------------------------- ----- 13.2/15.5 MB 2.6 MB/s eta 0:00:01
       ---------------------------------- ----- 13.4/15.5 MB 2.6 MB/s eta 0:00:01
       ----------------------------------- ---- 13.8/15.5 MB 2.6 MB/s eta 0:00:01
       ------------------------------------ --- 14.1/15.5 MB 2.7 MB/s eta 0:00:01
       ------------------------------------ --- 14.3/15.5 MB 2.7 MB/s eta 0:00:01
       ------------------------------------- -- 14.5/15.5 MB 2.8 MB/s eta 0:00:01
       -------------------------------------- - 14.8/15.5 MB 2.8 MB/s eta 0:00:01
       -------------------------------------- - 15.1/15.5 MB 2.9 MB/s eta 0:00:01
       ---------------------------------------  15.2/15.5 MB 2.9 MB/s eta 0:00:01
       ---------------------------------------  15.5/15.5 MB 3.0 MB/s eta 0:00:01
       ---------------------------------------- 15.5/15.5 MB 3.0 MB/s eta 0:00:00
    Downloading pytz-2024.1-py2.py3-none-any.whl (505 kB)
       ---------------------------------------- 0.0/505.5 kB ? eta -:--:--
       ----------------------- ---------------- 297.0/505.5 kB 6.1 MB/s eta 0:00:01
       ---------------------------------------- 505.5/505.5 kB 5.3 MB/s eta 0:00:00
    Downloading regex-2023.12.25-cp312-cp312-win_amd64.whl (268 kB)
       ---------------------------------------- 0.0/268.9 kB ? eta -:--:--
       ---------------------------------------- 268.9/268.9 kB 8.1 MB/s eta 0:00:00
    Downloading joblib-1.3.2-py3-none-any.whl (302 kB)
       ---------------------------------------- 0.0/302.2 kB ? eta -:--:--
       ---------------------------------------  297.0/302.2 kB 9.2 MB/s eta 0:00:01
       ---------------------------------------- 302.2/302.2 kB 6.2 MB/s eta 0:00:00
    Downloading tqdm-4.66.2-py3-none-any.whl (78 kB)
       ---------------------------------------- 0.0/78.3 kB ? eta -:--:--
       ---------------------------------------- 78.3/78.3 kB ? eta 0:00:00
    Installing collected packages: pytz, tqdm, regex, numpy, joblib, pandas, nltk
    Successfully installed joblib-1.3.2 nltk-3.8.1 numpy-1.26.4 pandas-2.2.1 pytz-2024.1 regex-2023.12.25 tqdm-4.66.2
    


```python
#import neccessary libraries
import pandas as pd
import nltk
```


```python
#load the dataset and indicate python that the JSON files is separated by lines!
df = pd.read_json("C:\\Users\\Administrator\\Downloads\\train_rand_split.jsonl", lines=True)
```


```python
#Check if the data was loaded OK
df.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>answerKey</th>
      <th>id</th>
      <th>question</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>A</td>
      <td>075e483d21c29a511267ef62bedc0461</td>
      <td>{'question_concept': 'punishing', 'choices': [...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>B</td>
      <td>61fe6e879ff18686d7552425a36344c8</td>
      <td>{'question_concept': 'people', 'choices': [{'l...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>A</td>
      <td>4c1cb0e95b99f72d55c068ba0255c54d</td>
      <td>{'question_concept': 'choker', 'choices': [{'l...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>D</td>
      <td>02e821a3e53cb320790950aab4489e85</td>
      <td>{'question_concept': 'highway', 'choices': [{'...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C</td>
      <td>23505889b94e880c3e89cff4ba119860</td>
      <td>{'question_concept': 'fox', 'choices': [{'labe...</td>
    </tr>
  </tbody>
</table>
</div>




```python
#display what columns you have in yoyr data frame
print(df.columns)
```

    Index(['answerKey', 'id', 'question'], dtype='object')
    


```python
from nltk.tokenize import word_tokenize
nltk.download('punkt')  # Download the NLTK tokenizer data

```

    [nltk_data] Downloading package punkt to
    [nltk_data]     C:\Users\Administrator\AppData\Roaming\nltk_data...
    [nltk_data]   Unzipping tokenizers\punkt.zip.
    




    True




```python
df['question'] = df['question'].apply(word_tokenize)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[14], line 1
    ----> 1 df['question'] = df['question'].apply(word_tokenize)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\series.py:4915, in Series.apply(self, func, convert_dtype, args, by_row, **kwargs)
       4780 def apply(
       4781     self,
       4782     func: AggFuncType,
       (...)
       4787     **kwargs,
       4788 ) -> DataFrame | Series:
       4789     """
       4790     Invoke function on values of Series.
       4791 
       (...)
       4906     dtype: float64
       4907     """
       4908     return SeriesApply(
       4909         self,
       4910         func,
       4911         convert_dtype=convert_dtype,
       4912         by_row=by_row,
       4913         args=args,
       4914         kwargs=kwargs,
    -> 4915     ).apply()
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\apply.py:1427, in SeriesApply.apply(self)
       1424     return self.apply_compat()
       1426 # self.func is Callable
    -> 1427 return self.apply_standard()
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\apply.py:1507, in SeriesApply.apply_standard(self)
       1501 # row-wise access
       1502 # apply doesn't have a `na_action` keyword and for backward compat reasons
       1503 # we need to give `na_action="ignore"` for categorical data.
       1504 # TODO: remove the `na_action="ignore"` when that default has been changed in
       1505 #  Categorical (GH51645).
       1506 action = "ignore" if isinstance(obj.dtype, CategoricalDtype) else None
    -> 1507 mapped = obj._map_values(
       1508     mapper=curried, na_action=action, convert=self.convert_dtype
       1509 )
       1511 if len(mapped) and isinstance(mapped[0], ABCSeries):
       1512     # GH#43986 Need to do list(mapped) in order to get treated as nested
       1513     #  See also GH#25959 regarding EA support
       1514     return obj._constructor_expanddim(list(mapped), index=obj.index)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\base.py:921, in IndexOpsMixin._map_values(self, mapper, na_action, convert)
        918 if isinstance(arr, ExtensionArray):
        919     return arr.map(mapper, na_action=na_action)
    --> 921 return algorithms.map_array(arr, mapper, na_action=na_action, convert=convert)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\algorithms.py:1743, in map_array(arr, mapper, na_action, convert)
       1741 values = arr.astype(object, copy=False)
       1742 if na_action is None:
    -> 1743     return lib.map_infer(values, mapper, convert=convert)
       1744 else:
       1745     return lib.map_infer_mask(
       1746         values, mapper, mask=isna(values).view(np.uint8), convert=convert
       1747     )
    

    File lib.pyx:2972, in pandas._libs.lib.map_infer()
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\__init__.py:129, in word_tokenize(text, language, preserve_line)
        114 def word_tokenize(text, language="english", preserve_line=False):
        115     """
        116     Return a tokenized copy of *text*,
        117     using NLTK's recommended word tokenizer
       (...)
        127     :type preserve_line: bool
        128     """
    --> 129     sentences = [text] if preserve_line else sent_tokenize(text, language)
        130     return [
        131         token for sent in sentences for token in _treebank_word_tokenizer.tokenize(sent)
        132     ]
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\__init__.py:107, in sent_tokenize(text, language)
         97 """
         98 Return a sentence-tokenized copy of *text*,
         99 using NLTK's recommended sentence tokenizer
       (...)
        104 :param language: the model name in the Punkt corpus
        105 """
        106 tokenizer = load(f"tokenizers/punkt/{language}.pickle")
    --> 107 return tokenizer.tokenize(text)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1281, in PunktSentenceTokenizer.tokenize(self, text, realign_boundaries)
       1277 def tokenize(self, text: str, realign_boundaries: bool = True) -> List[str]:
       1278     """
       1279     Given a text, returns a list of the sentences in that text.
       1280     """
    -> 1281     return list(self.sentences_from_text(text, realign_boundaries))
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1341, in PunktSentenceTokenizer.sentences_from_text(self, text, realign_boundaries)
       1332 def sentences_from_text(
       1333     self, text: str, realign_boundaries: bool = True
       1334 ) -> List[str]:
       1335     """
       1336     Given a text, generates the sentences in that text by only
       1337     testing candidate sentence breaks. If realign_boundaries is
       1338     True, includes in the sentence closing punctuation that
       1339     follows the period.
       1340     """
    -> 1341     return [text[s:e] for s, e in self.span_tokenize(text, realign_boundaries)]
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1329, in PunktSentenceTokenizer.span_tokenize(self, text, realign_boundaries)
       1327 if realign_boundaries:
       1328     slices = self._realign_boundaries(text, slices)
    -> 1329 for sentence in slices:
       1330     yield (sentence.start, sentence.stop)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1459, in PunktSentenceTokenizer._realign_boundaries(self, text, slices)
       1446 """
       1447 Attempts to realign punctuation that falls after the period but
       1448 should otherwise be included in the same sentence.
       (...)
       1456     ["(Sent1.)", "Sent2."].
       1457 """
       1458 realign = 0
    -> 1459 for sentence1, sentence2 in _pair_iter(slices):
       1460     sentence1 = slice(sentence1.start + realign, sentence1.stop)
       1461     if not sentence2:
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:321, in _pair_iter(iterator)
        319 iterator = iter(iterator)
        320 try:
    --> 321     prev = next(iterator)
        322 except StopIteration:
        323     return
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1431, in PunktSentenceTokenizer._slices_from_text(self, text)
       1429 def _slices_from_text(self, text: str) -> Iterator[slice]:
       1430     last_break = 0
    -> 1431     for match, context in self._match_potential_end_contexts(text):
       1432         if self.text_contains_sentbreak(context):
       1433             yield slice(last_break, match.end())
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1395, in PunktSentenceTokenizer._match_potential_end_contexts(self, text)
       1393 previous_slice = slice(0, 0)
       1394 previous_match = None
    -> 1395 for match in self._lang_vars.period_context_re().finditer(text):
       1396 
       1397     # Get the slice of the previous word
       1398     before_text = text[previous_slice.stop : match.start()]
       1399     index_after_last_space = self._get_last_whitespace_index(before_text)
    

    TypeError: expected string or bytes-like object, got 'dict'



```python
df['tokenized_question'] = df['question'].apply(word_tokenize)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[15], line 1
    ----> 1 df['tokenized_question'] = df['question'].apply(word_tokenize)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\series.py:4915, in Series.apply(self, func, convert_dtype, args, by_row, **kwargs)
       4780 def apply(
       4781     self,
       4782     func: AggFuncType,
       (...)
       4787     **kwargs,
       4788 ) -> DataFrame | Series:
       4789     """
       4790     Invoke function on values of Series.
       4791 
       (...)
       4906     dtype: float64
       4907     """
       4908     return SeriesApply(
       4909         self,
       4910         func,
       4911         convert_dtype=convert_dtype,
       4912         by_row=by_row,
       4913         args=args,
       4914         kwargs=kwargs,
    -> 4915     ).apply()
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\apply.py:1427, in SeriesApply.apply(self)
       1424     return self.apply_compat()
       1426 # self.func is Callable
    -> 1427 return self.apply_standard()
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\apply.py:1507, in SeriesApply.apply_standard(self)
       1501 # row-wise access
       1502 # apply doesn't have a `na_action` keyword and for backward compat reasons
       1503 # we need to give `na_action="ignore"` for categorical data.
       1504 # TODO: remove the `na_action="ignore"` when that default has been changed in
       1505 #  Categorical (GH51645).
       1506 action = "ignore" if isinstance(obj.dtype, CategoricalDtype) else None
    -> 1507 mapped = obj._map_values(
       1508     mapper=curried, na_action=action, convert=self.convert_dtype
       1509 )
       1511 if len(mapped) and isinstance(mapped[0], ABCSeries):
       1512     # GH#43986 Need to do list(mapped) in order to get treated as nested
       1513     #  See also GH#25959 regarding EA support
       1514     return obj._constructor_expanddim(list(mapped), index=obj.index)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\base.py:921, in IndexOpsMixin._map_values(self, mapper, na_action, convert)
        918 if isinstance(arr, ExtensionArray):
        919     return arr.map(mapper, na_action=na_action)
    --> 921 return algorithms.map_array(arr, mapper, na_action=na_action, convert=convert)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\algorithms.py:1743, in map_array(arr, mapper, na_action, convert)
       1741 values = arr.astype(object, copy=False)
       1742 if na_action is None:
    -> 1743     return lib.map_infer(values, mapper, convert=convert)
       1744 else:
       1745     return lib.map_infer_mask(
       1746         values, mapper, mask=isna(values).view(np.uint8), convert=convert
       1747     )
    

    File lib.pyx:2972, in pandas._libs.lib.map_infer()
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\__init__.py:129, in word_tokenize(text, language, preserve_line)
        114 def word_tokenize(text, language="english", preserve_line=False):
        115     """
        116     Return a tokenized copy of *text*,
        117     using NLTK's recommended word tokenizer
       (...)
        127     :type preserve_line: bool
        128     """
    --> 129     sentences = [text] if preserve_line else sent_tokenize(text, language)
        130     return [
        131         token for sent in sentences for token in _treebank_word_tokenizer.tokenize(sent)
        132     ]
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\__init__.py:107, in sent_tokenize(text, language)
         97 """
         98 Return a sentence-tokenized copy of *text*,
         99 using NLTK's recommended sentence tokenizer
       (...)
        104 :param language: the model name in the Punkt corpus
        105 """
        106 tokenizer = load(f"tokenizers/punkt/{language}.pickle")
    --> 107 return tokenizer.tokenize(text)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1281, in PunktSentenceTokenizer.tokenize(self, text, realign_boundaries)
       1277 def tokenize(self, text: str, realign_boundaries: bool = True) -> List[str]:
       1278     """
       1279     Given a text, returns a list of the sentences in that text.
       1280     """
    -> 1281     return list(self.sentences_from_text(text, realign_boundaries))
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1341, in PunktSentenceTokenizer.sentences_from_text(self, text, realign_boundaries)
       1332 def sentences_from_text(
       1333     self, text: str, realign_boundaries: bool = True
       1334 ) -> List[str]:
       1335     """
       1336     Given a text, generates the sentences in that text by only
       1337     testing candidate sentence breaks. If realign_boundaries is
       1338     True, includes in the sentence closing punctuation that
       1339     follows the period.
       1340     """
    -> 1341     return [text[s:e] for s, e in self.span_tokenize(text, realign_boundaries)]
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1329, in PunktSentenceTokenizer.span_tokenize(self, text, realign_boundaries)
       1327 if realign_boundaries:
       1328     slices = self._realign_boundaries(text, slices)
    -> 1329 for sentence in slices:
       1330     yield (sentence.start, sentence.stop)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1459, in PunktSentenceTokenizer._realign_boundaries(self, text, slices)
       1446 """
       1447 Attempts to realign punctuation that falls after the period but
       1448 should otherwise be included in the same sentence.
       (...)
       1456     ["(Sent1.)", "Sent2."].
       1457 """
       1458 realign = 0
    -> 1459 for sentence1, sentence2 in _pair_iter(slices):
       1460     sentence1 = slice(sentence1.start + realign, sentence1.stop)
       1461     if not sentence2:
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:321, in _pair_iter(iterator)
        319 iterator = iter(iterator)
        320 try:
    --> 321     prev = next(iterator)
        322 except StopIteration:
        323     return
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1431, in PunktSentenceTokenizer._slices_from_text(self, text)
       1429 def _slices_from_text(self, text: str) -> Iterator[slice]:
       1430     last_break = 0
    -> 1431     for match, context in self._match_potential_end_contexts(text):
       1432         if self.text_contains_sentbreak(context):
       1433             yield slice(last_break, match.end())
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\nltk\tokenize\punkt.py:1395, in PunktSentenceTokenizer._match_potential_end_contexts(self, text)
       1393 previous_slice = slice(0, 0)
       1394 previous_match = None
    -> 1395 for match in self._lang_vars.period_context_re().finditer(text):
       1396 
       1397     # Get the slice of the previous word
       1398     before_text = text[previous_slice.stop : match.start()]
       1399     index_after_last_space = self._get_last_whitespace_index(before_text)
    

    TypeError: expected string or bytes-like object, got 'dict'



```python
df['stem'] = df['stem'].apply(word_tokenize)
```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\indexes\base.py:3805, in Index.get_loc(self, key)
       3804 try:
    -> 3805     return self._engine.get_loc(casted_key)
       3806 except KeyError as err:
    

    File index.pyx:167, in pandas._libs.index.IndexEngine.get_loc()
    

    File index.pyx:196, in pandas._libs.index.IndexEngine.get_loc()
    

    File pandas\\_libs\\hashtable_class_helper.pxi:7081, in pandas._libs.hashtable.PyObjectHashTable.get_item()
    

    File pandas\\_libs\\hashtable_class_helper.pxi:7089, in pandas._libs.hashtable.PyObjectHashTable.get_item()
    

    KeyError: 'stem'

    
    The above exception was the direct cause of the following exception:
    

    KeyError                                  Traceback (most recent call last)

    Cell In[16], line 1
    ----> 1 df['stem'] = df['stem'].apply(word_tokenize)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\frame.py:4090, in DataFrame.__getitem__(self, key)
       4088 if self.columns.nlevels > 1:
       4089     return self._getitem_multilevel(key)
    -> 4090 indexer = self.columns.get_loc(key)
       4091 if is_integer(indexer):
       4092     indexer = [indexer]
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\indexes\base.py:3812, in Index.get_loc(self, key)
       3807     if isinstance(casted_key, slice) or (
       3808         isinstance(casted_key, abc.Iterable)
       3809         and any(isinstance(x, slice) for x in casted_key)
       3810     ):
       3811         raise InvalidIndexError(key)
    -> 3812     raise KeyError(key) from err
       3813 except TypeError:
       3814     # If we have a listlike key, _check_indexing_error will raise
       3815     #  InvalidIndexError. Otherwise we fall through and re-raise
       3816     #  the TypeError.
       3817     self._check_indexing_error(key)
    

    KeyError: 'stem'



```python
df['stem'] = df['stem'].astype(str)

```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\indexes\base.py:3805, in Index.get_loc(self, key)
       3804 try:
    -> 3805     return self._engine.get_loc(casted_key)
       3806 except KeyError as err:
    

    File index.pyx:167, in pandas._libs.index.IndexEngine.get_loc()
    

    File index.pyx:196, in pandas._libs.index.IndexEngine.get_loc()
    

    File pandas\\_libs\\hashtable_class_helper.pxi:7081, in pandas._libs.hashtable.PyObjectHashTable.get_item()
    

    File pandas\\_libs\\hashtable_class_helper.pxi:7089, in pandas._libs.hashtable.PyObjectHashTable.get_item()
    

    KeyError: 'stem'

    
    The above exception was the direct cause of the following exception:
    

    KeyError                                  Traceback (most recent call last)

    Cell In[17], line 1
    ----> 1 df['stem'] = df['stem'].astype(str)
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\frame.py:4090, in DataFrame.__getitem__(self, key)
       4088 if self.columns.nlevels > 1:
       4089     return self._getitem_multilevel(key)
    -> 4090 indexer = self.columns.get_loc(key)
       4091 if is_integer(indexer):
       4092     indexer = [indexer]
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\indexes\base.py:3812, in Index.get_loc(self, key)
       3807     if isinstance(casted_key, slice) or (
       3808         isinstance(casted_key, abc.Iterable)
       3809         and any(isinstance(x, slice) for x in casted_key)
       3810     ):
       3811         raise InvalidIndexError(key)
    -> 3812     raise KeyError(key) from err
       3813 except TypeError:
       3814     # If we have a listlike key, _check_indexing_error will raise
       3815     #  InvalidIndexError. Otherwise we fall through and re-raise
       3816     #  the TypeError.
       3817     self._check_indexing_error(key)
    

    KeyError: 'stem'



```python
df['question'] = df['question'].astype(str)

```


```python
df['tokenized_question'] = df['question'].apply(word_tokenize)

```


```python
print(df.head())
```

      answerKey                                id  \
    0         A  075e483d21c29a511267ef62bedc0461   
    1         B  61fe6e879ff18686d7552425a36344c8   
    2         A  4c1cb0e95b99f72d55c068ba0255c54d   
    3         D  02e821a3e53cb320790950aab4489e85   
    4         C  23505889b94e880c3e89cff4ba119860   
    
                                                question  \
    0  {'question_concept': 'punishing', 'choices': [...   
    1  {'question_concept': 'people', 'choices': [{'l...   
    2  {'question_concept': 'choker', 'choices': [{'l...   
    3  {'question_concept': 'highway', 'choices': [{'...   
    4  {'question_concept': 'fox', 'choices': [{'labe...   
    
                                      tokenized_question  
    0  [{, 'question_concept, ', :, 'punishing, ', ,,...  
    1  [{, 'question_concept, ', :, 'people, ', ,, 'c...  
    2  [{, 'question_concept, ', :, 'choker, ', ,, 'c...  
    3  [{, 'question_concept, ', :, 'highway, ', ,, '...  
    4  [{, 'question_concept, ', :, 'fox, ', ,, 'choi...  
    


```python
df['tokenized_question'] = df['question'].apply(lambda tokens: ' '.join(tokens))

```


```python
print(df.head())
```


```python
print(df[['question', 'full_question']].head())
```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    Cell In[23], line 1
    ----> 1 print(df[['question', 'full_question']].head())
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\frame.py:4096, in DataFrame.__getitem__(self, key)
       4094     if is_iterator(key):
       4095         key = list(key)
    -> 4096     indexer = self.columns._get_indexer_strict(key, "columns")[1]
       4098 # take() does not accept boolean indexers
       4099 if getattr(indexer, "dtype", None) == bool:
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\indexes\base.py:6200, in Index._get_indexer_strict(self, key, axis_name)
       6197 else:
       6198     keyarr, indexer, new_indexer = self._reindex_non_unique(keyarr)
    -> 6200 self._raise_if_missing(keyarr, indexer, axis_name)
       6202 keyarr = self.take(indexer)
       6203 if isinstance(key, Index):
       6204     # GH 42790 - Preserve name from an Index
    

    File ~\AppData\Local\Programs\Python\Python312\Lib\site-packages\pandas\core\indexes\base.py:6252, in Index._raise_if_missing(self, key, indexer, axis_name)
       6249     raise KeyError(f"None of [{key}] are in the [{axis_name}]")
       6251 not_found = list(ensure_index(key)[missing_mask.nonzero()[0]].unique())
    -> 6252 raise KeyError(f"{not_found} not in index")
    

    KeyError: "['full_question'] not in index"

print(df[['question', 'question']].head())
print(df[['question', 'tokenized_question']].head())


```python
df['tokenized_question'] = df['question'].apply(word_tokenize)
```


```python
print(df.head())
```

      answerKey                                id  \
    0         A  075e483d21c29a511267ef62bedc0461   
    1         B  61fe6e879ff18686d7552425a36344c8   
    2         A  4c1cb0e95b99f72d55c068ba0255c54d   
    3         D  02e821a3e53cb320790950aab4489e85   
    4         C  23505889b94e880c3e89cff4ba119860   
    
                                                question  \
    0  {'question_concept': 'punishing', 'choices': [...   
    1  {'question_concept': 'people', 'choices': [{'l...   
    2  {'question_concept': 'choker', 'choices': [{'l...   
    3  {'question_concept': 'highway', 'choices': [{'...   
    4  {'question_concept': 'fox', 'choices': [{'labe...   
    
                                      tokenized_question  
    0  [{, 'question_concept, ', :, 'punishing, ', ,,...  
    1  [{, 'question_concept, ', :, 'people, ', ,, 'c...  
    2  [{, 'question_concept, ', :, 'choker, ', ,, 'c...  
    3  [{, 'question_concept, ', :, 'highway, ', ,, '...  
    4  [{, 'question_concept, ', :, 'fox, ', ,, 'choi...  
    


```python

```
