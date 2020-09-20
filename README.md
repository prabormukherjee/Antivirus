# Antivirus

Malware detection is a very useful problem. But it is not too hard, to get the solution, atleast when you have a large amount of data. Today I made a simple Antivirus(malware detector) using Machine Learning algorithm. It is nothing but a clasification problem i.e. whether our target is harmful(malware) or not.    

Now I got a few dataset which is quite useful. I'm using the dataset from Kaggle by Microsoft. The data is stored in md5 hashed value. You can check the original dataset which was more than 30 gb(compressed). I provided a small subset of this data if you want to try. To run it on your machine check all the dependency of my project. You have to have Numpy,Pandas, Sklearn, Pickle, PE file installed on your system. Make sure you are on Python3 environment. Still if you get any error download the dependency or can contact with me.    

You may get some warning on running this project. That is Deprication warning, which means some change may occur in future with this library. But don't worry about it, I'll change the source code if it breaks at any point. The warnings on
*   importing joblib from sklearn.externals which can be directly done by joblib module `pip install joblib`
*   using the value of n_estimators, because they will change the default value from 10 to 100    

The source code for Python is provided. All you have to do is clone(or manually download zip) file in your machine, then install the dependencies and finally run the training.py file. It will train the model. I used some popular classification algorithm to check which one is the best for this dataset. Then I showed the accuracy for each algo. For my dataset the best one was Random Forest with an accuracy of 94.8%, which is no doubt awesome. Then using Pickel and Joblib I saved the weight of my pretrained model. And finally I added a testing.py file which can test the algo on some random dataset.    

Some extra pyfile( data_generator and manager_chk) is added here for data generation and managing purpose. PE file is efficient to test several edge cases with malwares. Hashlib is a library to impliment some hashed functions(such as md5). So I keep this 2 file for any data generation. It will take the image automatically for the data.
