# Data Bias in Perspective API 
_By MacKenna Landry_

In this assignment, I addressed teh bias and fairness of the Perspective API's toxicity detection model. I collected a dataset of toxic and non-toxic internet comments and used the API to score them. The threshold for toxiticity classification was set at 0.5, which means scores greater than 0.5 are considered toxic, and scores below 0.5 were deemed non toxic. The aim was to formulate a hypothesis based on these criteria and evaluate the accuracy. 

## Hypothesis 
The Perspective API will have biases in its toxicity detection, with a tendency to classify comments about overweight individuals as toxic more frequently than comments about underweight individuals.

## Results 
Throughout this assignment, I gained valuable experience in data collection, working with APIs, machine learning, understanding biases, and improving my GitHub skills. I categorized my data into four groups:

1. Toxic comments towards the overweight class
2. Non Toxic comments towards the overweight class
3. Toxic comments towards the underweight class
4. Non Toxic comments towards the underweight class

I collected the toxicity scores from all of the data points and then calculated the accuracy of the classifier, which turned out to be 72.41%. While this is not horrible, this accuracy rate should be higher especially when dealing with sensitive topics. 

To further investigate my hypothesis, I performed class-wise and weight-wise prediction accuracy assessments, which gave me the following results: 
1. Category 1 Toxic Comments  (Overweight class)= 75%
2. Category 2 Non toxic comments (Overweight class) = 85.7%
3. Category 3 Toxic Comments(Underweight class) = 37.5%
4. Category 4 Non Toxic Comments (Underweight class)= 100%

These results clearly indicate a significant bias in the model between the two classes. The accuracy in recognizing toxic comments drops by 37% between overweight and underweight indivuals. This imbalance violates predictive equity and equal opportunity. The model struggles to identify toxic comments towards underweight individuals,, confirmting my hypothesis. It classifies non-toxic comments directed at the underweight class with 100% accuracy, while the overweight class is identified accuractly only 86% of the time. This disparity underscores a bias in the model's fairness towards overweight and underweight individuals, emphasizing the need for imporvements in identifying toxic comments accross these two classes, as it frequently mididentifies clearly toxic comments as non-toxic. 

Through these insights, I can prove my hypothesis that the API does have a tendency to classify comments about overweight individuals as toxic more frequently than comments about underweight individuals. 

   
