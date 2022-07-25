While looking at the dataset, we can clearly see that it is heavily biased and also require cleaning; 
•	Big disproportionality in the classes (about 80% of shoppers do not proceed with a purshase)
•	2 Missing months in months 
•	Useless data like browser and operating system (one could argue that these
 informations could be relevant for example giving us an idea of the wealth/buying capacity 
of the user but social phenomenons counters that argument ; those who are less wealthy try to fit in by 
bying more that they can afford while the wealthy try to get out of the box buying « uncommon » product, 
a good example of this phenomenon is Iphonnes. 
In this project we decided to not get too involved in the potential causation effect of each variable and jsut focus on the most important ones according to randomForest::importance()


In this code, we cleaned the data and then applied the following methods with special techniques including stratified data splitting and hyper tuning to tackle the problem from all directions
• Gaussian naïve bayes 
• Random Forest; this was our best performing model, one would expect 
that the deep learning model would perform better and it probably will , but our lack 
of knowledge and experience puts it at a disadvantage.
• Extra Trees 
• Logstic Model 
• Support Vector Machines（SVM） 
• Deep Learning ;


Our score was decent in the context of a machine learning problem, 
and even if it intuitively look like it has almost the same odds of a statistical model, 
90% model acc vs 85% if we just answer no every time, the use of stratified data and the comparison 
with the dummy model and the AUC score of 0.9 clearly shows that our model is better than luck.
