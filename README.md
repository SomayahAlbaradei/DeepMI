# DeepSTEMI
# 1.	Project Description: 
This research addresses the critical imperative for improved cardiac care in pre-hospital emergency services through the integration of an artificial intelligence (AI) based diagnostic system. A survey involving 237 participants in Saudi Arabia illuminates the essential need to minimize on-site duration during cardiac emergencies, with unanimous agreement among participants regarding the pivotal role of AI in expediting responses, also demographic analysis provides valuable insights into participant trends, contributing to a comprehensive background understanding. The study proposes a methodological pipeline that encompasses key elements, including data augmentation, ResNet50 model training, and the development of a user-friendly AI assistant named DeepSTEMI. This AI assistant is designed to predict specifically ST-segment elevation myocardial infarction (STEMI) from given images and respond to initial treatment. Demonstrating robust binary classification performance, the ResNet50 model consistently exhibits high precision, recall, F1-score, and accuracy. A validated area under the curve (AUC) score of 0.98 underscores the model's discriminative prowess in distinguishing STEMI from normal cases. Emphasizing practical strategies, the study advocates for collaboration with the Saudi Red Crescent Authority, continuous model refinement, and system expansion to address a broader spectrum of cardiac conditions. Furthermore, the research highlights the importance of integrating real-time data feeds and incorporating continuous learning as pivotal elements to enhance diagnostic precision.
# 2.	Installation Instructions:
 This project uses Anaconda v3 with Python 3.10 and Flask framework. Follow the steps below to set up the environment and run the application locally:
a.	Anaconda Installation:
•	Download and install Anaconda v3 from the official website: Anaconda Downloads.
b.	Create a Virtual Environment:
•	Open a terminal or command prompt.
•	Navigate to the project directory.
•	Run the following command to create a virtual environment (replace env_name with your preferred environment name):
	conda create --name env_name python=3.10 
c.	Activate the Virtual Environment:
•	Activate the virtual environment using the following command:
	conda activate env_name 
d.	Install Required Packages:
•	While in the activated virtual environment, install the necessary packages by running:
	conda install flask 
This will install Flask, the web framework used for the application.
e.	Download HTLM Templates:
•	Ensure that the HTML templates mentioned in the project are available in the appropriate directory.
f.	Execute the Jupyter Notebook (ipynb file):
•	Execute the provided Jupyter Notebook file (ipynb) to train the ResNet50 model.
•	After execution, a model.h5 file will be generated, containing the trained model.
g.	Build and Run the Flask Application:
•	Use the model.h5 file to build the Flask application. Ensure that the Flask application code references the correct path to the trained model.
•	Run the Flask application using the following command:
	flask run 
•	Open a web browser and go to http://localhost:5000 to access the locally hosted application.

3.	Usage: The application is designed to provide a straightforward experience for predicting cardiac conditions, specifically ST-segment elevation myocardial infarction (STEMI), from uploaded medical images. Follow these simple steps to use the application:
a.	Access the Application:
•	Ensure that the Flask application is running locally by executing the command:
	flask run 
•	Open your web browser and go to http://localhost:5000.
b.	Image Upload:
•	On the application's interface, locate the option to upload medical images.
•	Click the designated area or button to select and upload the image you want to analyze.
c.	Prediction Report:
•	Once the image is uploaded, the AI assistant (DeepSTEMI) will process the data using the trained ResNet50 model.
•	The application will generate a prediction report that includes:
•	The prediction result (STEMI or normal case).
•	Medical measures recommended based on the prediction.
•	Date and time of the analysis.
•	Other relevant information related to the prediction.
d.	Review the Results:
•	Examine the prediction report to understand the AI's assessment of the uploaded medical image.
•	Take note of the recommended medical measures provided in the report.
e.	Repeat as Needed:
•	You can upload multiple images for analysis.
•	Repeat the process for each image you want to assess.

Important Notes for Contribution:
•	Interpretation of Results:
•	Understand that the prediction is based on the AI model's analysis of the provided medical images. Consult with healthcare professionals for comprehensive medical advice.
•	Feedback and Improvement:
•	Provide feedback on the application's predictions to contribute to continuous model refinement.
•	Consider collaborating with healthcare professionals to enhance the accuracy and reliability of the diagnostic system.




![image](https://github.com/SomayahAlbaradei/DeepSTEMI/assets/23430033/1f837220-873d-49fd-9167-aa303893029f)

