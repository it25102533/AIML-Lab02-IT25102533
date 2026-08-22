<p align="center">
  <img src="/resources/sliit.png" alt="Alt text" width="120"/>
</p>

<h1 align="center">IT2011 - Artificial Intelligence and Machine Learning</h1>
<h2 align="center">Lab 02 - Introduction to Generative AI</h2>


## Objectives:  
* Learn about using different types of prompting styles
* Use OpenAI's API
* Calling Hugging Face and its APIs
* Additional Resources



## Exercise 1:
Use the provided AWS Academy Generative AI Foundations course provided https://awsacademy.instructure.com/courses/129069 and complete the two activities in Module 04 - Using prompts and prompt engineering 


<img src="/resources/lab.png" alt="Alt text" style="width: 50%;"/>


1. Provide Screen shots of you doing the two labs as evidence.
2. Submit your answers under Exercise 1

## Exercise 2:
Look at the LLM Leaderboard - https://artificialanalysis.ai/leaderboards/models

1. Where does your favourite LLM rank currently?
2. Try out at least two models that you haven't tried before (you will have to do a seperate google search to find these products)
3. Run two prompts of your choice
4. Submit the model, the prompt and the responses you have got.

## Exercise 3:
Use the following large language models, enabling the reasoning model of the platform and generate a detail report on "How you can use generative AI as a university student to learn subjects like probability and statistics, data base management systems and software engineering"

1. https://chat.deepseek.com - Deepthing R1
2. https://chat.qwen.ai - Thinking
3. https://x.com/i/grok - DeepSearch

In your submission, mention the LLMs used, the report, and a reflection of anything useful you have found, in your opinion which tool produced the best results

## Exercise 4:

1. In this lab we will use OpenAI API to develop an application in python
2. Create an account at https://www.deeplearning.ai
3. Register to the free course at https://learn.deeplearning.ai/courses/chatgpt-building-system
4. Select the second activity
   

<img src="/resources/lab02.png" alt="Alt text" style="width: 60%;"/>

4. Execute the first code line in Jupiter notebook
5. Add the following code and in a codeblock and run

```
# Define system prompt (initial behavior) 
system_prompt = {"role": "system", "content": "You are a helpful assistant with deep knowledge in physics."} 
 
# Define user prompt (specific query) 
user_prompt = {"role": "user", "content": "Explain how black holes are formed."} 
 
# Send prompt to API 
response = openai.ChatCompletion.create( 
    model="gpt-3.5-turbo", 
    messages=[system_prompt, user_prompt] 
) 
print(response['choices'][0]['message']['content'])
```
Please see the figure below if you have issues running this</br>

<img src="/resources/lab03.png" alt="Alt text" style="width: 45%;"/>



6. Copy the codeblock given above again to the next cell and perform the following changes
7. Give a System Prompt for a chatbot to behave as an expert event planner
8. Give a User Prompt asking for advice how to plan for an event you have to do, maybe your friends Birthday Party, or a Batch Outing
9. Tryout a unique System prompt and User Prompt for a problem of your choice.
10. Share screen shots and upload the prompts and responses for the above activities 

## Exercise 5.
1. Create an account in https://huggingface.co
2. Select any AI project of your liking under Spaces
3. Tryout the AI project and generate the output
4. Share screenshots of your usage of the AI project
5. Under Models select a Model of your choice to find more details about it
6. Create an account in https://colab.research.google.com
7. Change Runtime to GPU

<img src="/resources/lab04.png" alt="Alt text" style="width: 30%;"/>

9. Run the summarization example in a codeblock, here the Hugging Face open model will be downloaded to Google Colab and then it will be exectuted. Because of this it will take some time to run the model for the first time.




```
from transformers import pipeline
summarizer = pipeline("summarization")
summary = summarizer("""Hugging Face is a pioneering open-source AI platform
  that empowers developers, researchers, and organizations to easily access and
  deploy cutting-edge machine learning models for natural language processing, computer vision,
  and beyond—democratizing AI and accelerating innovation through a collaborative ecosystem of tools,
  datasets, and community-driven contributions.""", max_length=20)
print(summary)

```
10. Have a look at a specific summarization model available in HuggingFace - https://huggingface.co/EbanLee/kobart-summary-v3
11. Run the summarization for this model given below, here the Hugging Face open model will be downloaded to Google Colab and then it will be exectuted. Because of this it will take some time to run the model for the first time.

```
from transformers import pipeline

# Use a known summarization model
summarizer = pipeline("summarization", model="EbanLee/kobart-summary-v3")

# Input text to summarize
text = """Hugging Face is a pioneering open-source AI platform
that empowers developers, researchers, and organizations to easily access and
deploy cutting-edge machine learning models for natural language processing, computer vision,
and beyond—democratizing AI and accelerating innovation through a collaborative ecosystem of tools,
datasets, and community-driven contributions."""

# Generate summary
summary = summarizer(text, max_length=20, min_length=5, do_sample=False)
print(summary)
```
12. Select a Natural Language Model of your choice from Hugging Face

<img src="/resources/lab05.png" alt="Alt text" style="width: 30%;"/>

13. Try your best to see if you can get your selected Model running in Google CoLab.  In some instances you will have to install additional python libraries.
Some models have on the Right Side called Use this Model, where you can get Google CoLab code that you can try to use.
<img src="/resources/lab06.png" alt="Alt text" style="width: 25%;"/>
15. Attach screen shots of your solution running for 9, 11, and 13
16. Submit the code and the output for 13

## Exercise 6.
1. Create an Account in Coursera - https://www.coursera.org/
2. Register to these three courses</br></br>
https://www.coursera.org/learn/learning-chatgpt</br>
https://www.coursera.org/learn/prompt-engineering</br>
https://www.coursera.org/learn/learning-how-to-learn</br></br>
3. Select a topic from the Prompt Engineering Course given above, and develop your own prompt based on the style given
4. Try it out in your favourite LLM
5. Share the prompt, output and a screenshot of what you have done
6. Go through these courses when you have some free time
   
## Exercise 7.

1. Submit all lab work you have done, including screenshots based on instructions given to you.

   
<p align="center"><b>(c) Faculty of Computing, SLIIT</b></p>


