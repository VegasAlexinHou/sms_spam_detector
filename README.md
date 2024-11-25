# SMS Spam Detection Application

This repository contains code for a SMS spam detection application that classifies text messages as either spam or not spam using a linear Support Vector Classification (SVC) model. The application is hosted using Gradio, allowing users to input text messages and receive feedback on whether the message is classified as spam or not.

## Files

- `sms_text_classification_solution.ipynb`: Jupyter notebook containing the original code for training the SVC model on SMS text messages.
- `gradio_sms_text_classification.ipynb`: Jupyter notebook containing the refactored code to create the SVC model function and the Gradio interface for hosting the application.
- `Resources/SMSSpamCollection.csv`: Dataset containing SMS text messages used for training the model.

## SMS Classification Function

The `create_sms_classification_model` function in `gradio_sms_text_classification.ipynb` loads the SMS dataset, splits the data into training and testing sets, builds a pipeline to transform the data, fits the model, and returns the trained model.

## SMS Prediction Function

The `sms_prediction` function in `gradio_sms_text_classification.ipynb` takes a text message input, predicts the classification using the pre-trained model, and returns a message indicating whether the text message is spam or not.

## Gradio Interface Application

The Gradio interface application in `gradio_sms_text_classification.ipynb` allows users to input text messages and receive real-time feedback on whether the message is classified as spam or not. The application provides a clear and user-friendly interface for testing text messages.

## Usage

To use the application, simply run the code in `gradio_sms_text_classification.ipynb` to launch the Gradio interface. Users can input text messages and receive instant feedback on the classification.

## Testing

The application can be tested using the following text messages:
1. "You are a lucky winner of $5000!"
2. "You won 2 free tickets to the Super Bowl."
3. "You won 2 free tickets to the Super Bowl. Text us to claim your prize."
4. "Thanks for registering. Text 4343 to receive free updates on medicare."

## Dependencies

- pandas
- scikit-learn
- gradio

## Acknowledgements

This project was inspired by the need for an efficient SMS spam detection solution and was implemented using machine learning techniques and the Gradio library for hosting the application.

Everyone is free to explore the code and contribute to further improvements in SMS spam detection.
