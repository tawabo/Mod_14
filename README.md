# Mod_14

You’ll combine your new algorithmic trading skills with your existing skills in financial Python programming and machine learning to create an algorithmic trading bot that learns and adapts to new data and evolving markets.

In a Jupyter notebook, you’ll do the following:

Implement an algorithmic trading strategy that uses machine learning to automate the trade decisions.

Adjust the input parameters to optimize the trading algorithm.

Train a new machine learning model and compare its performance to that of a baseline model.



Technologies
You will load the following libraries 


<img width="587" alt="Import file 14" src="https://user-images.githubusercontent.com/95396568/161449294-2f51007a-de4e-460f-bf63-c5593873ee3a.png">


Usage
This section should include screenshots, code blocks, or animations explaining how to use your project.

<img width="610" alt="initial window" src="https://user-images.githubusercontent.com/95396568/161449319-d59db293-6163-4a60-9cb0-bec7aca71d52.png">
<img width="613" alt="initial train " src="https://user-images.githubusercontent.com/95396568/161449324-1b36f16b-7cfc-4c7c-8e2a-61c52fc13fa7.png">
<img width="649" alt="initial class" src="https://user-images.githubusercontent.com/95396568/161449333-386bfe63-1dc8-4033-b13a-5e79ba63b8c9.png">
The Initial Classification report came back with a decent average .5 macro and .55 weighted however -1 recall was pretty low


<img width="689" alt="Window C Class" src="https://user-images.githubusercontent.com/95396568/161449439-0dbbd0e0-cbc7-49e6-a1f9-0e6d607b2be4.png">
Changing the the Short to 8 and long to 50 basically removed all -1 from the data which caused to many false positives precision avg went down drastically


<img width="686" alt="6 monthclass" src="https://user-images.githubusercontent.com/95396568/161449568-c40af180-56de-4622-b662-139999178880.png">
By extending the DataOffset to 6 months it boosted the recall by a bit but dropped the precision very little the report was a bit more realistic then inital testing


<img width="658" alt="win 8 1" src="https://user-images.githubusercontent.com/95396568/161449660-d1734db8-0224-4554-a0e9-0e9704e1a0a5.png">
By expanding the short window to 8 and leaving the long window as is there was a very slight difference


<img width="647" alt="win 2" src="https://user-images.githubusercontent.com/95396568/161449697-17c09850-cb10-48ed-bd91-49543f396648.png">
Dropping the windows by half both short and long from initial data provided noticed that pboth precision and recall went up for -1.  With that being said the macro average and weighted average were also a bit more imporoved which shows that the average was a bit more realistic


