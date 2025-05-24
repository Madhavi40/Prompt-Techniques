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

###### Self-Consistency Prompting #####

Solve the following problem. Think step-by-step through 3 different possible reasoning paths.
Problem: “When I was 6, my sister was half my age. Now I'm 70. How old is my sister?"

Reasoning Path 1:

When I was 6, my sister was half my age, so she was 3 years old. The age difference between us is 6 - 3 = 3 years.
Now that I'm 70, my sister is 70 - 3 = 67 years old. 
Answer from Path 1: 67

Reasoning Path 2:
When I was 6 my sister was half my age, so she was 3. Now I am 70, so she is 70/2 = 35.
Answer from Path 2: 35.

Reasoning Path 3:
When I was 6, my sister was half my age, so she was 3 years old. The age difference between us is 6 - 3 = 3 years.
Now that I'm 70, my sister is 70 - 3 = 67 years old.
Answer from Path 3: 67

✅ Final Answer:
67 years old.

#### General Knowledge Prompting #####

Prompt:
Generate some knowledge about meditation, including its practices and general benefits. Then answer the question : What are the benefits of meditation?

Response:

What Is Meditation?
Meditation is a practice that involves focusing the mind to achieve a mentally clear and emotionally calm and stable state. It has been practiced for thousands of years in numerous religious traditions and beliefs, but it is not confined to any particular religion. Today, meditation is often used for stress reduction and relaxation.

Common Meditation Practices
. Mindfulness Meditation: Involves paying attention to thoughts, sounds, the sensations of breathing, or parts of the body without judgment.
. Transcendental Meditation: Involves silently repeating a mantra in a specific way.
. Guided Meditation: Involves meditating under the guidance of a teacher or recording, often involving visualization.
. Loving-kindness Meditation (Metta): Focuses on developing feelings of goodwill, kindness, and warmth towards others.

Benefits of Meditation
Meditation offers a wide array of benefits, encompassing mental, emotional, and physical well-being:

. Reduces Stress: Meditation helps activate the body's relaxation response, reducing the production of stress hormones and promoting a sense of calm and relaxation.
. Enhances Emotional Health: Regular meditation can improve emotional stability and promote a positive outlook. It can help manage and control emotions more effectively.
. Improves Concentration: Meditation can enhance focus, concentration, and cognitive performance by training the mind to stay in the present and redirecting attention.
. Promotes Physical Health: Research suggests that meditation can have a positive impact on physical health by lowering blood pressure, improving sleep quality, boosting the immune system, and reducing inflammation in the body.
. Cultivates Mindfulness and Self-Awareness: Meditation fosters a state of mindfulness, allowing individuals to observe their thoughts, feelings, and sensations without judgment.This heightened self-awareness can lead to greater self-understanding and personal growth.

✅ Final Answer
Meditation is a versatile practice that can significantly enhance various aspects of life. By incorporating meditation into daily routines, individuals can experience improved mental clarity, emotional stability, and overall well-being.

