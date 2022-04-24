# Perform A/B Testing 

### A/B Testing Use Case
A/B tests are very commonly performed by data analysts and data scientists. For this project, you will be working to understand the results of an A/B test run by an e-commerce website.  Your goal is to work through this notebook to help the company understand if they should:
- Implement the new webpage, 
- Keep the old webpage, or 
- Perhaps run the experiment longer to make their decision.


## Summary of Findings

Findings from the experimentations done with the data provided of the webpage visitations :
- An A/B test was performed from scratch
Since a timestamp is associated with each event, you could run a hypothesis test continuously as long as you observe the events. 

However, then the hard questions would be: 
- Do you stop as soon as one page is considered significantly better than another or does it need to happen consistently for a certain amount of time?  
- How long do you run to render a decision that neither page is better than another?  
 Some observations:
  - What is this value called in scientific studies?  
 - What does this value signify in terms of whether or not there is a difference between the new and old pages? *Hint*: Compare the value above with the "Type I error rate (0.05)". 
- This value that I computed is called p-value.
- It signifies if the decision we took is correct on not, Our assumption was that the null and alternative hypothesis were equal. Now the computed p-value is 0.903 which is greater than 0.05 , so we can conclude that failed to reject the null. The new page is no better than the old page. 
- Also the negative observed difference suggests that the old_page may be slightly better.



- Performing the Null Hypothesis testing using built in functions we got a similar result as from scratch.

- In the final part the same A/B test was performed using a regression approach.
Observations:

- Including both page and country had no significant effect on conversion, because of statistically insignific.
- Part 3 results suggest that country and treatment are not having much of a significance on the prediction of conversion rates. 
- The old_page performance was calculated to be slightly better than the new page. Which leads to a conclusion that the company should consider running the test for longer to get a more diverse dataset which maybe topple the favors in preferrence of new_page. Or , maybe some other factor that we might not have thought of until now, which could have an influence on conversion rates.
