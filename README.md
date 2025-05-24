**Prompt Techniques:

##### Zero-Hot Prompting #######
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

pic

###### Meta Prompting ########


