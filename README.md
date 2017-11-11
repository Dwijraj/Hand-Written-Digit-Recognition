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
			1182 sec= 20mins
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(accuracy_score)
		</td>
		<td>
			92
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(accuracy_score)
		</td>
		<td>
			92
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			< 1sec 
		</td>	
	</tr>
</table>

<h2>Hand Written Data Recognition Using KNN alogorithm.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into sklearn's KNNClassifier and the following observations were recorded<br/>
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
			18secs
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(accuracy_score)
		</td>
		<td>
			92.8
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(accuracy_score)
		</td>
		<td>
			97.4
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			64sec = 1 mins
		</td>	
	</tr>
</table>
<h2>Hand Written Data Recognition Using SVC.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into sklearn's Support Vector Machine Classifier and the following observations were recorded<br/>
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
			620secs =18mins
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(accuracy_score)
		</td>
		<td>
			94.864
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(accuracy_score)
		</td>
		<td>
			93.1
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			259sec = 4 mins
		</td>	
	</tr>
</table>
<h2>Hand Written Data Recognition Using GaussianNB.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into sklearn's Gaussian Naive Bayes and the following observations were recorded <br/>
<table>
	<caption>Observation</caption>
	<tr>
		<td>
			Classifier Properties
		</td>
		<td>
			GaussianNB(priors=None)
		</td>
	</tr>
	<tr>
		<td>
			Training Time
		</td>
		<td>
			0.50 seconds
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(accuracy_score)
		</td>
		<td>
			55.212
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(accuracy_score)
		</td>
		<td>
			55.54
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			1 sec
		</td>	
	</tr>
</table>	
<h2>Hand Written Data Recognition Using NeuralNetwork.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into a neural network implemented in tensorflow and the following observations were recorded <br/>
<table>
	<caption>Observation</caption>
	<tr>
		<td>
			Classifier Properties
		</td>
		<td>
			total_layers=7
			Layer_Units={1:38,2:38,3:38,4:38,5:38,6:38,7:10}
			Activation functions for layer 1-6 ReLU
			Activatioin function for output layer Softmax
			Optimizer used :- Adam Optimizer 
			Learning rate:- 0.001
			Steps used :- 1500
			Training type:- Full batch
		</td>
	</tr>
	<tr>
		<td>
			Training Time
		</td>
		<td>
			2820.50 seconds= 47mins
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(tf.metrics.accuracy)
		</td>
		<td>
			99.7
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(tf.metrics.accuracy)
		</td>
		<td>
			99.2
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			< 1 sec
		</td>	
	</tr>	
</table>
<h2>Hand Written Data Recognition Using ConvolutionNeuralNetwork.ipynb</h2>
Simple script in which data is used from the generated pickle files and then 
fed into a neural network(with CNN) implemented in tensorflow and the following observations were recorded <br/>
<table>
	<caption>Observation</caption>
	<tr>
		<td>
			Classifier Properties
		</td>
		<td>
			total_layers=3
			Layer_1(Convolutional layer with maxpool) (CNN(kernel=[4,4,1,8],strides=[1,1,1,1],padding='SAME' )->ReLU-> Maxpooling(padding='SAME',ksize=[1,8,8,1],strides=[1,8,8,1]))
			Layer_2(Convolutional layer with maxpool) (CNN(kernel=[2,2,8,16],strides=[1,1,1,1],padding='SAME' )->ReLU-> Maxpooling(padding='SAME',ksize=[1,4,4,1],strides=[1,4,4,1]))
			Layer_3(Fully Connected Classifier)(Neurons =10, <strong>NO ACTIVATION FUNCTION</strong>)
			Optimizer used :- Adam Optimizer 
			Learning rate:- 0.001
			Steps used :- 1500
			Training type:- Full batch
		</td>
	</tr>
	<tr>
		<td>
			Training Time
		</td>
		<td>
			14646 seconds= 244mins=4hrs
		</td>
	</tr>
	<tr>
		<td>
			Training Accuracy(tf.metrics.accuracy)
		</td>
		<td>
			95
		</td>
	</tr>
	<tr>
		<td>
			Testing Accuracy(tf.metrics.accuracy)
		</td>
		<td>
			95
		</td>	
	</tr>
	<tr>
		<td>
			Testing time
		</td>
		<td>
			< 1 sec
		</td>	
	</tr>	
</table>
<h2>Hand Written Data Recognition in NeuralNetwork using Keras.ipynb</h2>
<p>
	Same neural network as <h2>Hand Written Data Recognition Using NeuralNetwork.ipynb</h2> 
	implemented in Keras
</p>	