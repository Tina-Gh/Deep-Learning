<strong>Notes:</strong>

<a href="https://www.superdatascience.com/pages/deep-learning" target="_blank">Super Data Sciene</a>
<html>
<body>
<p>Different Deep Learning Methods and their applications:</p>

<table style="width:100%">
  <tr>
    <th>Deep Learning Method</th>
    <th>Application</th> 
  </tr>
  <tr>
    <td>ANN</td>
    <td>Used for Regression and Classification</td>
  </tr>
  <tr>
    <td>CNN</td>
    <td>Used for Computer Vision</td>
  </tr>
  <tr>
    <td>RNN</td>
    <td>Used for Time Series Analysis</td>
  </tr>
  <tr>
    <td>Self-Organizing Maps (SOM)</td>
    <td>Used for Feature Detection</td>
  </tr>
  <tr>
    <td>Deep Boltzmann Machines</td>
    <td>Used for Recommendation systems</td>
  </tr>
  <tr>
    <td>AutoEncoders</td>
    <td>Used for Recommendation systems</td>
  </tr>
</table>

</body>

# Deep-Learning-Python-codes
Here, I put my Deep learning related python codes: (This section is under construction! I am working on updating this documentry.)

<br>
<b>*CNN_malaria_cells_images_project.ipynb:</b>

Detecting if cells are infected by Malaria or not based on a Convolutional Neural Netwok. The dataset can be downloaded from the <a href="https://lhncbc.nlm.nih.gov/publication/pub9932">National Library of Medicine</a>. In addition, since it takes quite a long time for the model to be fit, I used a pre-defined trained file named "malaria_detector.h5" that I have also uploaded here.

<br>
<b>*02-Autoencoder-Exercise_UK foods.ipynb:</b>

The dataset is "UK_foods.csv", and this code detects a country in the Uk that their food and meals are more distictive than the rest.

<br>
<b>*02-RNN-Exercise_Ice cream and frozen dessert dataset.ipynb:</b>

The dataset can be found from <a href="https://fred.stlouisfed.org/series/IPN31152N">Industrial Production: Nondurable Goods: Ice cream and frozen dessert</a>

<hr>

<strong>* 10_RNN_google stock dataset_Regression:</strong>

The dataset is "Google_Stock_Price_Train.csv" and "Google_Stock_Price_Test.csv". In this code I built a model using RNN to predict the Google's stock prices for January 2017, given the dataset from 2012 to 2016. The model could well follow the upward and the downward trends.

here are different ways to improve the RNN model:
<ol>
  <li>Getting more training data: we trained our model on the past 5 years of the Google Stock Price but it would be even better to train it on the past 10 years.</li>
  <li>Increasing the number of timesteps: the model remembered the stock prices from the 60 previous financial days to predict the stock price of the next day. That’s because we chose a number of 60 timesteps (3 months). You could try to increase the number of timesteps, by choosing for example 120 timesteps (6 months).</li>
  <li>Adding some other indicators: if you have the financial instinct that the stock price of some other companies might be correlated to the one of Google, you could add this other stock price as a new indicator in the training data.</li>
  <li>Adding more LSTM layers: we built a RNN with four LSTM layers but you could try with even more.</li>
  <li>Adding more neurones in the LSTM layers: we highlighted the fact that we needed a high number of neurones in the LSTM layers to respond better to the complexity of the problem and we chose to include 50 neurones in each of our 4 LSTM layers. You could try an architecture with even more neurones in each of the 4 (or more) LSTM layers.</li>
</ol>

<br>
<strong>* 14_SOM_fraud detection.ipynb:</strong>

<a href="http://www.ai-junkie.com/ann/som/som1.html" target="_blank">ai-junkie!</a>

The dataset is "Credit_Card_Applications.csv". This dataset is the <a href="http://archive.ics.uci.edu/ml/support/statlog+(australian+credit+approval)" target="_blank">UCI's Statlog (Australian Credit Approval)</a> dataset. The fraudulent client IDs are specified at the end of the code.
<ul>
  <li>SOMs retain topology of the input set</li>
  <li>SOMs reveal correlations that are not easily identified (feature detection)</li>
  <li>SOMs classify data without supervision (unsupervised learning)</li>
  <li>No target vector -> No backpropagation</li>
  <li>No lateral connections between output nodes</li>
</ul>

<br>
<strong>* 15_SOM_Mega Case Study.ipynb:</strong>

The dataset is "Credit_Card_Applications.csv". This is continuing the "14_SOM_fraud detection.ipynb" code in a hybrid mode, i.e. not only implementing a SOM (Self-Organizing maps) model but also implementing an ANN model afterwards to predict the probabilty of conducting fraudulant activity for all the Client IDs!

<br>
<strong>* 16_Boltzmann Machine_Recommender system.ipynb</strong>

<a href="https://pytorch.org/docs/master/" target="_blank">PyTorch documentation</a>

(Comming soon!)
