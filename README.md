 #  **Analyze Google Play Store Apps Data**
 


<img width="1000" height="400" src="Figures/googleplay2.png">


<li><a href="#Overview">Overview</a></li>
<li><a href="#Data Description">Data Description</a></li>
<li><a href="#Objectives">Objectives</a></li>
<li><a href="#Libraries">Libraries</a></li>
<li><a href="#Results">Results</a></li>
<li><a href="#References">References</a></li>
<li><a href="#Acknowledgments">Acknowledgments</a></li>

<a id='Overview'></a>
## Overview:
- Language 
  > Python
- Environment
  > [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb)
- Data Source
  > [Kaggle](https://www.kaggle.com/) 

<a id='Data Description'></a>
## Data Description:
- ### Google Play Store Apps [Dataset](https://www.kaggle.com/lava18/google-play-store-apps)  
  - **Details Of Data** :
     - App: Application name

     - Category: Category the app belongs to

     - Rating: Overall user rating of the app 

     - Reviews: Number of user reviews for the app 

     - Size: Size of the app 

     - Installs: Number of user downloads/installs for the app

     - Type: Paid or Free

     - Price: Price of the app 

     - Content Rating: Age group the app is targeted at - Children / Mature 21+ / Adult

     - Genres: An app can belong to multiple genres (apart from its main category)

     - Last Updated: Date when the app was last updated on Play Store

     - Current Ver: Current version of the app available on Play Store

     - Android Ver: Min required Android version

<a id='Objectives'></a>
## Objectives:
  1. To Find The Most And Least Popular `Category` In Google Play Store .

  2. To Find What The Kind Of `Content Rating` That Most Apps Belong To In Google Play Store .

  3. Finding The Ratio Of `Paid` To `Free` Apps In Google Play Store .

  4. Find Out If There Is A Relationship Between Apps `Reviews` And `Rating` In Google Play Store .

  5. To Find Out The Most Frequently Used Value For `Rating` Apps In Google Play Store .

<a id='Libraries'></a>
## Libraries:
- **Environment Setting** 
  > - **warnings** : ignore warning message
  > - **google.colab.files** : download plots 
- **Data Manipulation**
  > - **pandas** : data manipulation
  > - **numpy** : numerical operations
  > - **math** : mathematical operations 
  > - **preprocessing** : encoding operations 
- **Visualization**
  > - **matplotlib.pyplot** : visualizing data 
  > - **seaborn** : visualizing data and colors palette 
  > - **plotly.graph_objects** : interactive visualize data
- **Modeling**
  > - **sklearn.model_selection.train_test_split** : data separation to train and test 
  > - **sklearn.model_selection.GridSearchCV** : optimize score
  > - **sklearn.linear_model.LinearRegression** :  linear regression modeling
  > - **sklearn.metrics.r2_score** : getting r2_score
  > - **sklearn.metrics.mean_squared_error** : getting mean squared error
  > - **sklearn.metrics.mean_absolute_error** : getting mean absolute error
   
   
<a id='Results'></a>
## Results:
-  ### **EDA Results**
 _______________________________________________________________________________________
   -<img width="700" height="350" src="Figures/Category Sort (2).bmp"/>
   #### **- The Most Popular Categories In The App Store Are Family And Games ,And The Least Popular Are Beauty Apps.**
 _______________________________________________________________________________________
   -<img width="600" height="600" src="Figures/ContentRatingCount.png">
   #### **- Almost All The Apps Target "Everyone", With A Ratio Of (81.8%).**
 _______________________________________________________________________________________
   -<img width="600" height="600" src="Figures/AppsType.png">
   #### **- Most Of Apps In This Store Are Free , With A Ratio Of (92.2%).**
 _______________________________________________________________________________________
   -<img width="700" height="400" src="Figures/ReviewsVSRating.png">
   #### **- There Is A Positive Relationship Between The Reviews And The Ratings Of Apps.**
 _______________________________________________________________________________________
   -<img width="700" height="400" src="Figures/RatingVSApps.png">
   #### **- The Most Frequntly Value To Rating The Apps Is 4.5 With '5199 App'.**
 _______________________________________________________________________________________
 ### **Also, You can find an intractive plots Inside the [colab notebook](https://colab.research.google.com/gist/ShaimaM/8ff4896a007ef811447e70d7f46e7207/untitled10.ipynb#scrollTo=FtCM4tSFPDRC)..**
_______________________________________________________________________________________


- ### **Model Results**

   - ### **Linear Regression:** 
   #### **The best possible R2 score is `0.93` , With** 
    > **`32.8` MAE**
    
    > **`24.0` MSE**
    
    > **`1.08` RMSE**
    #### **And The model results are unchanged from the previous one after tuning GridsearchCV.**
   - ### **Baseline Result:** 
    > **`82.3` MAE**
    #### **Tha result of MAE increased from `32,8` to `82.3`.**

<a id='References'></a>
## References:
- [scikit-learn](https://scikit-learn.org/stable/) 
- [Matplotlib](https://matplotlib.org/stable/index.html) 
- [Seaborn](https://seaborn.pydata.org/) 
- [Plotly](https://plotly.com/python/) 

<a id='Acknowledgments'></a>
## Acknowledgments:
 ### This project was supported by the **Saudi Digital Academy**, for the Data Science Bootcamp. 
  **Done By: Shaima Mohammed Alamri**

