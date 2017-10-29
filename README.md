# Hand-Written-Digit-Recognition
This is a repository with various classifier written in jupyter notebook that works on hand written digits images.The data set can be downloaded
from <a href='https://drive.google.com/open?id=0B4OCp-_lGauXLVJsdl9zZ3NIZUk'>this</a> link.
Download the zip file and extract all the images before running ipynb files and also
 <strong>Hand Written Data Recognition Using Logistic Regression.ipynb</strong> 
should be run first so that pickle files are created

<h2>Hand Written Data Recognition Using Logistic Regression.ipynb</h2>

This is a jupyter notebook that reads images converts them into numpy array using 
scipy's ndimage and then each digit's pickle file is created
pickle files are easy way to store python objects and also they are very fast to work with
Now the data can be easily load for other scripts as 
well.These data are then fed LogisticRegression classifier using sklearn
The following observations were noted
<table>
	<caption>Observation</caption>
	<tr>
		<td>
			Classifier Properties
		</td>
		<td>
			LogisticRegressionCV(Cs=10, class_weight=None, cv=None, dual=False,
			fit_intercept=True, intercept_scaling=1.0, max_iter=100,
			multi_class='ovr', n_jobs=1, penalty='l2', random_state=None,
			refit=True, scoring=None, solver='lbfgs', tol=0.0001, verbose=0)
		</td>
	</tr>
	<tr>
		<td>
			Training Time
		</td>
		<td>
			2215 sec = 36mins
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(accuracy_score)
		</td>
		<td>
			81.772
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(accuracy_score)
		</td>
		<td>
			81.64
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			5sec 
		</td>	
	</tr>
</table>

<h2>Hand Written Data Recognition Using KNN alogorithm.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into sklearn's KNNClassifier and the following observations were recorded
<table>
	<caption>Observation</caption>
	<tr>
		<td>
			Classifier Properties
		</td>
		<td>
			KNeighborsClassifier(algorithm='auto', leaf_size=30, metric='minkowski',
            metric_params=None, n_jobs=1, n_neighbors=5, p=2,
            weights='uniform')
		</td>
	</tr>
	<tr>
		<td>
			Training Time
		</td>
		<td>
			15secs
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(accuracy_score)
		</td>
		<td>
			85.902
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(accuracy_score)
		</td>
		<td>
			85.57
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			545sec = 9 mins
		</td>	
	</tr>
</table>
<h2>Hand Written Data Recognition Using SVC.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into sklearn's Support Vector Machine Classifier and the following observations were recorded
<table>
	<caption>Observation</caption>
	<tr>
		<td>
			Classifier Properties
		</td>
		<td>
			SVC(C=1.0, cache_size=200, class_weight=None, coef0=0.0,
				decision_function_shape='ovr', degree=3, gamma='auto', kernel='rbf',
				max_iter=-1, probability=False, random_state=None, shrinking=True,
				tol=0.001, verbose=False)
		</td>
	</tr>
	<tr>
		<td>
			Training Time
		</td>
		<td>
			15secs
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(accuracy_score)
		</td>
		<td>
			85.902
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(accuracy_score)
		</td>
		<td>
			85.57
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			545sec = 9 mins
		</td>	
	</tr>
</table>