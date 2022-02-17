# Chatbot_NN

In this project, I have created a Chatbot using intents data found on Kaggles. I have used NLP for data processing and Neural Networks to train the model on training data.   

# Data:
The data is in a JSON file and looks like below:    

{"intents": [.      
        {"tag": "greeting",     
         "patterns": ["Hi there", "How are you", "Is anyone there?","Hey","Hola", "Hello", "Good day"],      
         "responses": ["Hello, thanks for asking", "Good to see you again", "Hi there, how can I help?"],     
         "context": [""].    
        }.    
}.    
 
Where,   

**tag:** greetings is the class label.   
**patterns** represent words assigned to the respective tag.    

There are 9 classes in the dataset : 'adverse_drug', 'blood_pressure', 'blood_pressure_search', 'goodbye', 'greeting', 'hospital_search', 'options', 'pharmacy_search', 'thanks'.    

# For Training:    
Created NN model with three layers.    
1st - 128 neurons.   
2nd - 64 neurons    
3rd - output layer contains number of neurons equal to number of intents to predict output intent with softmax (9 classes).   
