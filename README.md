
</p>
<h2>Price Predictor of US Used Cars</h2>
<h2>Tool to help determine your car's current market value</h2>

<p>
<strong>Abstract</strong>
</p>
<p>
This work has been carried out with the objective of defining and implementing a
tool for determining the price of used cars that can be used by all professional
and non-professional users who enter the used car market in the United States.
With the analysis and subsequent training of the dataset, it has been possible
to predict the price that a used car has on the market with high percentages of
success. Likewise, the work concludes with the creation of an API that makes it
easier to carry out the requests that the user needs, according to the endpoint
created.
</p>

<p>
</p>
<p>
</p>
<p>
<span style="text-decoration:underline;">Table of contents</span>
</p>
<ol>
<strong>Dataset</strong>
</li>
</ol>
<p>
The study will be carried out based on the dataset of used vehicles from :
</p>
<p>
<em>Used Cars Dataset-Vehicles listings from Craigslist.org </em>from
<em>https://www.kaggle.com/</em>
</p>
<p>
Craigslist is the world's largest collection of used vehicles for sale, and this
dataset include
</p>
<ul>
<li>License CC0: Public Domain
<li>Last updated: 2021-05-06

<strong>Methodology</strong>  
<p>
In this project I will follow the CRISP-DM methodology. The Cross Industry
Standard Process for Data Mining (CRISP-DM) is a process model with six phases
that naturally describes the data science life cycle. It’s like a set of guides
to help you plan, organize, and implement your data science project.
</p>
<ol>
<li>Business understanding – What does the business need?
<li>Data understanding – What data do we have/need? Is it clean?
<li>Data preparation – How do we organize the data for modeling?
<li>Modeling – What modeling techniques should we apply?
<li>Evaluation – Which model best meets the business objectives?
<li>Deployment – How do stakeholders access the results?

<h2>Deployment</h2>
<p>
In order to prepare the model for productization, two aspects have been created.
On the one hand, the prediction function has been written that can be executed
in Jupyter Notebook  and with which the results can already be obtained in a
production environment.
</p>
<p>
 And on the other hand, an API has been developed with FastAPI technology so
that the pickel file can be implemented in any other App in such a way that the
functioning of the model is not compromised and it can evolve in successive
versions while always serving the user. Username. In this way, a third party can
use the WEB service and charge for a subscription or a call within a SaaS
framework with the developed model.
</p>
<ol>
</ol>
</li>
</ol>
<p>
</p>
<ol>
<h2>Productize the model</h2>
</li>
</ol>
<p>
</p>
<p>
From this point, with the model ready to be used in production, it can be easily
integrated into any web service facility that can be charged for its use.
Likewise, the update itself can be done easily without the need to change
anything in the frontend, forms and web pages. The API has been created to admit
a request in Jason format so that the way of building it is independent and the
request to the API is standardized.
</p>
<p>
</p>

<p>
<h2>The conclusions of this work are the following:</h2>
</p>
<ul>
<li>The model that has presented the best performance is the model obtained with
the XGboost algorithm.
<li>The tree-based algorithms are the ones that have had the best behaviour.
<li>More than 10 iterations with different combinations of variables,
techniques, algorithms have been necessary to achieve this performance,
exceeding 93.9% of the R2 score.
<li>The most important features, the ones that most influence splits in the
processing construction model, are Odometer, cylinders, fuel, drive and
manufacturer.
<li>It has been very important during the data preparation process to make the
decision not to generate dummies since it is based on categorical variables with
thousands of classes. This made it unfeasible to have a good Score since the
number of records per variable was very low. The transformation was carried out
with a Label encoder so that most of the classes of categorical variables could
be used. Among other issues, since the classes were well represented, it did not
seem to make sense to eliminate the car models or the car manufacturers, since
these would be crucial information for the user who later wanted to make
requests to the model. I would always have that data and the model should have
worked with most of it.
<li>During the cleaning process, subsets of the original dataset have been
outlined, so that the best score was obtained without losing too much data.
<li>Just as several variables have been eliminated, new variables (age, n_sold)
have also been created, which are ultimately the ones that have most influenced
the score.
<li>The application of neural networks, within the framework of Depp learning,
dense networks for the regression problem that we have has come out very
satisfactorily, and the author is left with the idea that very probably, with an
improvement in the amount of data or a For a more exhaustive search of the best
layer configurations, the neural networks would supersede the tree-like
algorithms of machine learning.
<li>The productization of the model is essential to answer the question of what
it is for, and I highlight the "get prices" function that has been developed in
the Jupiter notebook to generate the prediction since it includes the necessary
dictionaries for the correct interpretation by of the algorithm.
<li>The API has been created with the FastAPI library, very common and fast
among machine learning users, which facilitates the automatic generation of
endpoint documentation for implementation by third parties.
</li>
</ul>
<p>
</p>
<p>
<strong>References</strong>
</p>
<ul>
<li>Kaggle,Used Cars Dataset.Vehicles listings from Craigslist.org.(2016)
<p>
        <a
href="https://www.kaggle.com/austinreese/craigslist-carstrucks-data/metadat">https://www.kaggle.com/austinreese/craigslist-carstrucks-data/metadata</a>
</p>
<ul>
<li><a href="https://stackoverflow.com/">https://stackoverflow.com/</a>
<li><a
href="https://www.cienciadedatos.net/">https://www.cienciadedatos.net/</a>

</ul>
<p>
</p>


    
