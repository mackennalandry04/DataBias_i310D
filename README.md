# Data Bias in Perspective API 
_By MacKenna Landry_

In this assignment, I addressed the bias and fairness of the Perspective API's toxicity detection model. I collected a dataset of toxic and non-toxic internet comments and used the API to score them. The threshold for toxiticity classification was set at 0.5, which means scores greater than 0.5 are considered toxic, and scores below 0.5 were deemed non toxic. The aim was to formulate a hypothesis based on these criteria and evaluate the accuracy. Throughout this assignment, I gained valuable experience in data collection, working with APIs, machine learning, understanding biases, and improving my GitHub skills. 

## Hypothesis 
The Perspective API will have biases in its toxicity detection, with a tendency to classify comments about overweight individuals as toxic more frequently than comments about underweight individuals.

## Results 
I categorized my data into four groups:

1. Toxic comments towards the overweight class
2. Non Toxic comments towards the overweight class
3. Toxic comments towards the underweight class
4. Non Toxic comments towards the underweight class

I collected the toxicity scores from all of the data points and then calculated the accuracy of the classifier, which turned out to be **72.41%**. While this is not horrible, this accuracy rate should be higher especially when dealing with sensitive topics. 

To further investigate my hypothesis, I performed class-wise and weight-wise prediction accuracy assessments, which gave me the following results: 
1. Category 1 Toxic Comments  (Overweight class)= 75%
2. Category 2 Non toxic comments (Overweight class) = 85.7%
3. Category 3 Toxic Comments(Underweight class) = 37.5%
4. Category 4 Non Toxic Comments (Underweight class)= 100%

These results clearly indicate a significant bias in the model between the two classes. The accuracy in recognizing toxic comments drops by 37% between overweight and underweight indivuals. This imbalance violates predictive equity and equal opportunity. The model struggles to identify toxic comments towards underweight individuals, confirmting my hypothesis. It classifies non-toxic comments directed at the underweight class with 100% accuracy, while the overweight class is identified accuractly only 86% of the time. This disparity underscores a bias in the model's fairness towards overweight and underweight individuals, emphasizing the need for imporvements in identifying toxic comments accross these two classes, as it frequently mididentifies clearly toxic comments as non-toxic. 

Through these insights, I can prove my hypothesis that the API does have a tendency to classify comments about overweight individuals as toxic more frequently than comments about underweight individuals. Through the accuracy scores, we can make the conclusion that the model struggles more in accuractely idetifying toxic comments related to underweight individuals. 

Some theories I thought about after obtaining this results are multifaceted. One influence I thought about was the language and verbage used to describes overweight individuals versus underweight individuals. Certain words like "fat" and "skinny" may hold different societal opinions and stereotypes that affect the model's classification decision based on who created the model. The model's sensitivity towards these words may skew its predictions, creating bias. Another point I thought about was the training of the data/model. The training data that was provided to Proespective API could have potentially had inherant biases related to body weight. Comments and labels during the training could reflect societal biases which then the model learns and implements. Overall, I was surprised 
by these results, but sadly, societal biases and opinions are a very prevelant thing in our world. We will have to work on training the model to not have inherent bias.  

## Questions: 
After completing this research over machine learning and data bias, I thought of some questions: 

- What is the root cause of bias in data models and how can we identify it?
- Can we create bias mitigration strategies and implement them?
- Are there legal implications for biased models like this? 

