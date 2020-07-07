# Anitvirus

Malware detection is a very useful problem. But honestly speaking it is not too hard, atleast when you have a large amount of data. Today I made a simple Antivirus(malware detector) using Machine Learning algorithm. If you think logically, it is nothing but a clasification problem i.e. whether our target is harmful(malware) or not.
<br>
Now I got a few dataset which is quite useful. I'm using the dataset from Kaggle by Microsoft. The data is stored in md5 hashed value. You can check the original dataset which was more than 20 gb(compressed). I provided a small subset of this data if you want to try. To run it on your machine check all the dependency of my project. You have to have Numpy,Pandas, Sklearn, Pickle, PE file installed on your system. Make sure you are on Python3 environment. Still if you get any error download the dependency or can contact with me.
<br>
You may get some warning on running this project. That is Deprication warning, which means some change may occur in future with this library. But don't worry about it, I'll change the source code if it breaks at any point. The warnings on
<ul>
  <li> importing joblib from sklearn.externals which can be directly done by joblib module [pip install joblib] </li>
  <li> using the value of n_estimators, because they will change the default value from 10 to 100 </li>
</ul>

<br>
