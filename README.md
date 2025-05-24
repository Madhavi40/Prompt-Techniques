**Prompt Techniques:

##### Zero-Shot Prompting #######
Sentiment Analysis:
Analyze the sentiment of the following statement as positive, negative or neutral: 'The movie was fantastic!'
Sentiment:
output - positive

other examples of zero shot prompting use cases:
Summarization 
Question Answering
Medical Diagnosis 
Treatment Planning 
Intent Classification  
Multilingual Translation 
Text Summarization

##### Few-Shot Prompting ######

Classify the sentiment of the following text as positive, negative, or neutral.
Text: The product is terrible. Sentiment: Negative
Text: Super helpful, worth it. Sentiment: Positive
Text: It doesnt work! Sentiment:
output - Negative

###### Chain-of-Thought (CoT) Prompting ######

Zero-shot CoT Prompt:
"If I have 15 oranges and I give away 7 oranges, how many oranges do I have left? Let's think step-by-step."
Model Output:
"First, you start with 15 oranges. Then you give away 7, so you have 15 - 7 = 8 oranges left

Few-Shot Approaches:
Prompt: "Joe has 5 tennis balls. He buys 2 cans of tennis balls, each containing 3. How many tennis balls does he have now? Provide a chain of thought for your reasoning." 
Response: "Roger started with 5 balls. 2 cans of 3 tennis balls each is 6 tennis balls. 5 + 6 = 11." 

Automated Chain-of-Thought (Auto-CoT):

<img width="551" alt="auto CoT" src="https://github.com/user-attachments/assets/7d2e327c-9cfe-4cf8-8f3c-a23b779ab175" />


###### Meta Prompting ########

Prompt:
------
"Let's solve this math problem step by step. But before you start, think about how you would approach this problem logically. Then, proceed with your reasoning.

Question:
If a train travels 60 miles per hour for 2 hours, how far does it travel?

Instructions:
1. Reflect on the problem and consider the best approach to solve it.
2. Break down the problem into smaller, manageable steps.
3. Provide your final answer after completing the steps."

Expected Model Response:
-----------------------
"To solve this, I first think about the relationship between speed, time, and distance. The formula to calculate distance is:
Distance = Speed × Time
Now, applying the values:
Distance = 60 miles/hour × 2 hours = 120 miles
So, the train travels 120 miles."

🔍 What Makes It "Meta"?
In this example, the prompt explicitly asks the model to reflect on its reasoning process before proceeding with the solution. This meta-cognitive step encourages the model to consider its approach, potentially leading to more accurate and thoughtful responses.

✅ Benefits of Meta CoT Prompting
Enhanced Accuracy: By reflecting on the reasoning process, the model may identify and correct potential errors before arriving at a final answer.
Improved Transparency: This approach makes the model's thought process more explicit, aiding in understanding how it arrives at conclusions.
Better Problem-Solving: Encouraging reflection can lead to more effective strategies for tackling complex problems.

