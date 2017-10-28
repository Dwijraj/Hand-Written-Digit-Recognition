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
</table>

<h2>Hand Written Data Recognition Using KNN alogorithm.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into sklearn's KNNClassifier and the following observations were recorded
<table>
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
</table>