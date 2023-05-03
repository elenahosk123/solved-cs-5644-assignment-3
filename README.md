Download Link: https://assignmentchef.com/product/solved-cs-5644-assignment-3
<br>
(50 points) ​<strong>Regression; </strong>​Consider the Bike Share dataset from the UCI machine learning repository (<u>​</u><a href="https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset">https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset</a><u>​</u><a href="https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset">)</a>. The dataset contains three files, viz. ​<em>day.csv, hour.csv, </em>​and ​<em>Readme.txt. </em>​Both the datasets (data.csv and hour.csv) contain a combination of integer-valued (e.g., season, weekday or not) and real-valued features (e.g., temperature, windspeed). Details of the dataset are described in the README (​<em>Readme.txt</em>​) in the ​<em>Data Characteristics </em>​section. Just like the previous assignment, spend some time understanding the structure of the dataset, how the instances are organized, how the features are organized, what the various features mean (info in README), what features are useful for the task at hand, and so on. Do not attempt to run any machine learning algorithm before understanding the structure of the dataset.




Note, in particular, the last three fields in the data, viz. <strong><em>casual </em></strong>​          ​<em>(denotes casual riders), <strong>registered </strong></em>​<em>(registered riders), and </em>​<strong><em>cnt </em></strong>​<em>(total ridership count). </em>

<em> </em>

<ol>

 <li>Using only hour.csv, implement regression algorithms (both linear and k-nearest neighbors) to predict the hourly values for:

  <ol>

   <li>the number of casual riders</li>

   <li>the number of registered riders</li>

  </ol></li>

</ol>

<ul>

 <li>total ridership count</li>

</ul>




<ol>

 <li>Using only ​<em>csv</em>​, implement regression algorithms (both linear and k-nearest neighbors) to predict the daily values for:

  <ol>

   <li>the number of casual riders</li>

   <li>the number of registered riders</li>

  </ol></li>

</ol>

<ul>

 <li>total ridership count</li>

</ul>

Therefore, for each dataset, you are reporting 3 models for linear regression and 3 models for KNN regression.




<strong>Note: </strong>​Remember that using one of the target values (as a feature) in predicting the outcome of any of the counts – casual, registered, or total would defeat the purpose of the learning algorithm. It will make the problem too easy. That is, the number of ​<strong><em>casual </em></strong>riders cannot be used as a feature to predict the number of ​<strong>registered </strong>​riders or ​<strong>total </strong>ridership. Similarly, the number of ​<strong>registered </strong>​riders cannot be used to predict the other two values, and so on. Only features like season, temperature, real-feel, etc. have to be used by the learning algorithm.




For instance, suppose you are using ​<em>hourly.csv </em>​dataset and you want to predict the

number of ​<strong>casual </strong>​riders. You have to remove the columns related to the number of <strong>registered </strong>riders and ​       ​<strong>total </strong>​ridership first and then start training/testing your model. Similarly, when you are making the prediction model for ​<strong>total </strong>​ridership, you have to remove the columns related to <strong>casual </strong>​             ​rides and <strong>registered </strong>​              riders first and then start​            training/testing your model.




As before, you will need to separate the data into training set and test set (decide on the proportion of splits yourself). Evaluate the performance of your regression using suitable measures. Report on the performance results and which model(s) worked best (and why in your opinion).




<ol start="2">

 <li>(50 points) ​<strong>Clustering; </strong>​Consider the Seeds data set from the UCI machine learning repository (<a href="https://archive.ics.uci.edu/ml/datasets/seeds">https://archive.ics.uci.edu/ml/datasets/seed</a><u>​ </u><a href="https://archive.ics.uci.edu/ml/datasets/seeds">s</a>​). The dataset comprises of features from three different types of wheat kernels. There are seven features (area, perimeter, compactness, length, width, asymmetry coefficient, and length of kernel groove) that describe each data point. (Note that the dataset has an eighth column (​<em>class information with labels 1, 2, and 3</em>​), which we will use as ground truth to verify our clustering results.)</li>

</ol>




Using the ​<strong><em>k-means </em></strong>​algorithm cluster this dataset into three clusters based on the seven features at your disposal. Demonstrate the effectiveness of your implementation by comparing the results against the ground truth. Follow the steps in the k-means demo video from the lectures.




Also note that the default label values in scikit learn start from ​<strong><em>0</em></strong>​, whereas the dataset here starts labels with <strong><em>1</em></strong>​ ​. While evaluating your implementation’s effectiveness, ensure to account for this discrepancy.




As a performance measure, compare the clusters identified by k-means w.r.t. the ground truth data and make observations.




<strong>What to submit: </strong>

A zipped file containing:

<ol>

 <li>a PDF document summarizing answers to questions 1 and 2. Instead distill your lessons and experiences succinctly.</li>

 <li>Either hyperlinks to or actual attachments of your data files and your iPython notebook(s).</li>

</ol>











