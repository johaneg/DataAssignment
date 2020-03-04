# DataAssignment


# Anamnes - [Medical history](https://en.wikipedia.org/wiki/Medical_history)

First and foremost, thank you for taking your time to be part of our goal, to impact 1 000 000 000 (One billion) people. Everything we do is focused on this goal and to reach it we need people like __you__!

The medical team at [doctrin](http://doctrin.se/en/) are always looking for new ways to improve healthcare. Through years of practicing medicine they have become experts of listening and talking to patients. In this process they also learnt to ask the right questions about a patients condition and medical history.

The medical team hires __you__ as they heard that __you__ are a motivated and excellent problemsolver, they need you to build functioning prototype of their system.


## Requirements

Before each patient appointment they want the patient to fill in a questionnaire. The questionnaire will help the doctors before and during the appointment to give the best possible treatment. In order to follow up on how the questionnaires are used they want help to analyze event data.

1. Every anamnesis will be tagged with a unique id, and every event has an anamnesis id
1. Three different actions occur, "start_anamnesis", "question" and "end_anamnesis"
1. The question event will be have a field called question populated with the question and answer

### The questions for fever
 
1.	What was the last measured temperature
	1.	35 to 42 degrees.

2. How long have you had a fever?
	1. 0 to 14 days

3. Do you have any of the following. (radiobuttons, must activly select no)

	1. Problem breathing
	2. Stiff neck
	3. Chest pain
	4. abdominal pain

4. Do you have any of the following? (checkboxes)

	1. Sore throat
	2. Cough
	3. Muscle pain
	4. Vomiting

5. Have you recently traveled abroad? (radiobuttons)
	1. Yes
	2. No

### The task

These events, such as start/end anamnesis, and question are stored in raw json-files, see the anamnesis_events.zip.

1.  Instead of having the information stored by event we want the data grouped by anamnesisId, the transformed format could be json, csv or other. Each anamnesis_id, should have the start_time, end_time, anamnesis_completed (True or False), #unique_questions_answered, questions+answers (list with questions and answers) sorted by time.

1. Also there should be a function that counts the number of anamneses with a fever between values two values. The data used could be either the raw json data files or transformed data.

1. There should also be a function that counts the number of anamnesis with both "Stiff Neck", "Chest pain" but have not traveled abroad. The data used could be either the raw json data files or transformed data.


### The output

The output should be code that can be run in any environment, you don't have to include your transformed data, but it should be able to run the code and generate the transformed data and also run the two other functions. Please provide simple instructions if needed. You can choose what language you use. Also provide us with a short descriptions of what you have done, what you would do if you had more time and any assumptions you made. 


