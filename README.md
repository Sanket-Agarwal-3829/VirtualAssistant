Pharmacy Virtual Assistant
This project is a Pharmacy Virtual Assistant designed to classify customer queries and perform inventory actions based on the classification. It includes two major components:

Query Classification: A machine learning model that classifies text-based queries (e.g., "cancel order", "check inventory") using natural language processing techniques.
Voice Assistant: A voice-activated assistant using libraries like speech_recognition, pyttsx3, and more for natural interaction with users.
Features
Part 1: Query Classification & Inventory Management
Dataset of Queries: A dataset containing customer queries, each labeled with a corresponding action class (e.g., "cancel_order", "check_inventory").
Text Preprocessing: Uses CountVectorizer and TfidfVectorizer to transform the textual data into numerical form.
Model: Trained a classification model using MultinomialNB (Naive Bayes) from sklearn to predict the action based on customer input.
Inventory Management: Based on the classified query, the system interacts with the pharmacy’s inventory (e.g., cancel an order, check stock, or update inventory).
Part 2: Voice-Activated Assistant
Speech Recognition: Uses speech_recognition to convert spoken queries into text.
Text-to-Speech: Uses pyttsx3 to provide spoken responses.
Command Execution: Integrates with pywhatkit, wikipedia, and datetime to execute various voice commands like playing a song, fetching information, or checking the time.
Entertainment: Includes pyjokes to tell jokes on demand.
How It Works
Part 1: Query Classification
Data Preprocessing:

The dataset of queries is vectorized using CountVectorizer or TfidfVectorizer to convert the text into a numerical form suitable for machine learning.
Training the Model:

A MultinomialNB model from sklearn.naive_bayes is trained on the vectorized data to classify input queries into predefined categories.
Inventory Actions:

Once a query is classified (e.g., "cancel_order"), the assistant performs the appropriate action, such as updating the pharmacy's inventory or managing orders.
Part 2: Voice-Activated Assistant
Voice Input:

The system listens for user input via the microphone using the speech_recognition library and converts the speech to text.
Command Processing:

If the command is a general request (e.g., "play a song" or "tell me a joke"), the assistant processes it using:
pywhatkit to play music or videos.
wikipedia to search for information.
pyjokes for jokes.
datetime for time-related queries.
Voice Output:

The response is generated using the pyttsx3 text-to-speech engine, allowing the assistant to respond to the user verbally.
Libraries Used
Query Classification:
sklearn.feature_extraction.text.CountVectorizer
sklearn.feature_extraction.text.TfidfVectorizer
sklearn.naive_bayes.MultinomialNB
Voice Assistant:
speech_recognition – for recognizing speech.
pyttsx3 – for text-to-speech conversion.
pywhatkit – for handling media and web-based commands.
datetime – to handle date and time queries.
wikipedia – to fetch information from Wikipedia.
pyjokes – to tell jokes.
