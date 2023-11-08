# DataBias_i310D
## MacKenna Landry 

In this assignment, we are testing the the bias and fairness of the pre-existing Perspective API model. I created/found toxic and non toxic internet comments and the API gave them a score. For our testing, the threshold is 0.5; any scores greater than 0.5 are considered toxic and any scores below 0.5 are considered non toxic. We were to choose a hypothesis based on these conditions and then test the accuracy of the model. 

## Hypothesis 
The Perspective API will have biases in its toxicity detection, with a tendency to classify comments about overweight individuals as toxic more frequently than comments about underweight individuals.

## Results 
Through this assignment, I learned a lot about collecting data, APIs, biases, and improving my skills at using gitHub. I chose to put my data into four categories
1. Toxic comments towards the overweight class
2. Non Toxic comments towards the overweight class
3. Toxic comments towards the underweight class
4. Non Toxic comments towards the underweight class

   
With these datapoints I was able to calculate the accuracy of the classifier and this came out to be 72.41% accurate. This is not absolutely horrible, but should be better especially with sensitive topics.

After cacluating this, I needed to know more about the specific categories to officially investigate my hypothesis. So then I performed the class wise and weight wise prediction accuracy. After doing this I got these results: 
1. Category 1 Toxic Comments  (Overweight class)= 75%
2. Category 2 Non toxic comments (Overweight class) = 85.7%
3. Category 3 Toxic Comments(Underweight class) = 37.5%
4. Category 4 Non Toxic Comments (Underweight class)= 100%

From this, we can see that the model is heavily biased between the two classes. The accuracy of recognizing toxic comments drops 37% between overweight and underweight individuals. This definitely violated predictive equity and is against equal opportunity. It has a very difficult time recognizing toxic comments toward underweight people and identifying them as toxic. This is concerning and actually proves my hypothesis to be true. I hypothesized that the model would identify overweight comments as toxic more often then they would towards underweight individuals. Non-toxic comments directed at the underweight class are identified with 100% accuracy, while the overweight class is only accurately identified 86% of the time. This discrepancy further proves a bias in the model's fairness towards overweight and underweight individuals. This proves that the API will need work in idetifying toxic comments between these two classes as it commonly misidentifies clearly toxic comments as nontoxic.
   
