# BBC-News-Classification-using-hugging-face
classify news  into five categories: business, entertainment, politics, sport, and tech. 

Introduction: <br/>
The task of the project was to classify news articles into five categories: business, entertainment, politics, sport, and tech.<br/> The BBC News dataset was used for this task, which contains 2,225 articles from the BBC News website from 2004 to 2005.
<br/>
Preprocessing: <br/>
The dataset was loaded using the datasets library, and the text was cleaned by removing punctuations and stopwords.<br/> The text was then tokenized using the Hugging Face tokenizer and the labels were one-hot encoded. The tokenized articles were split into training and validation sets, and the model was fine-tuned on the training set.
<br/>
Architecture and Fine-tuning:<br/>
The pre-trained BERT model was used as the architecture for the text classification task.<br/> The model was fine-tuned on the tokenized articles using the Adam optimizer, a learning rate of 2e-5, and a batch size of 32. The model was trained for 5 epochs, and a checkpoint was saved after each epoch.
<br/>
Evaluation:<br/>
The trained model was evaluated on the validation set using accuracy, precision, recall, and F1-score metrics. <br/>The model achieved an accuracy of 97.7%, precision of 97.9%, recall of 97.7%, and an F1-score of 97.7%.
<br/>
Discussion:<br/>
The model achieved high accuracy on the validation set, indicating that it is performing well on this particular dataset.<br/> However, it is possible that the model may not perform as well on other datasets or real-world data. Possible ways to improve the model could be to increase the size of the training set, use a different pre-trained model architecture, or try different hyperparameters.
<br/>
Sample Predictions:<br/>
Here are a few sample predictions made by the trained model:
<br/>
Text: "The new iPhone is set to be released next month."<br/>
Predicted label: tech<br/>
Text: "The government has proposed a new tax policy."<br/>
Predicted label: politics<br/>
Text: "The latest movie from Steven Spielberg has received mixed reviews." <br/>
Predicted label: entertainment <br/>
Text: "The Manchester United soccer team won the game yesterday." <br/>
Predicted label: sport <br/>
Text: "The company has announced record profits for the year." <br/>
Predicted label: business <br/>
These predictions demonstrate that the model is able to accurately classify news articles into their corresponding categories.
<br/>




