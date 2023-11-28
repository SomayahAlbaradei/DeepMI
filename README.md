
# DeepSTEMI: Artificial Intelligent Support System for Rapid Diagnosis and Treatment of ST-segment elevation Myocardial Infarction in Pre-hospital Emergency Medical Services at SRCA In Makkah Al-Mukarramah

This research addresses the critical imperative for improved cardiac care in pre-hospital emergency services through the integration of an artificial intelligence (AI) based diagnostic system. A survey involving 237 participants in Saudi Arabia illuminates the essential need to minimize on-site duration during cardiac emergencies, with unanimous agreement among participants regarding the pivotal role of AI in expediting responses, also demographic analysis provides valuable insights into participant trends, contributing to a comprehensive background understanding. The study proposes a methodological pipeline that encompasses key elements, including data augmentation, ResNet50 model training, and the development of a user-friendly AI assistant named DeepSTEMI. This AI assistant is designed to predict specifically ST-segment elevation myocardial infarction (STEMI) from given images and respond to initial treatment. Demonstrating robust binary classification performance, the ResNet50 model consistently exhibits high precision, recall, F1-score, and accuracy. A validated area under the curve (AUC) score of 0.98 underscores the model's discriminative prowess in distinguishing STEMI from normal cases. Emphasizing practical strategies, the study advocates for collaboration with the Saudi Red Crescent Authority, continuous model refinement, and system expansion to address a broader spectrum of cardiac conditions. Furthermore, the research highlights the importance of integrating real-time data feeds and incorporating continuous learning as pivotal elements to enhance diagnostic precision.




## Installation

This project uses Anaconda v3 with Python 3.10 and Flask framework. Follow the steps below to set up the environment and run the application locally:
1. Anaconda Installation: 
Download and install Anaconda v3 from the official website: https://www.anaconda.com/download

2. Create a Virtual Environment:

2.1. Open a terminal or command prompt.

2.2. Navigate to the project directory.

2.3. Run the following command to create a virtual environment (replace env_name with your preferred environment name):

```bash
conda create --name env_name python=3.10 
```

3. Activate the virtual environment:

3.1. •	Activate the virtual environment using the following command:

```bash
conda activate env_name 
```

4. Install Required Packages:

4.1. While in the activated virtual environment, install the necessary packages by running

```bash
conda install flask  
```

5. Download HTLM templates:

5.1. •	Ensure that the HTML templates mentioned in the project are available in the appropriate directory

6. Execute the Jupyter Notebook (ipynb file):

6.1. Execute the provided Jupyter Notebook file (ipynb) to train the ResNet50 model

6.2. After execution, a model.h5 file will be generated, containing the trained model

7. Build and Run the Flask Application:

7.1. Use the model.h5 file to build the Flask application. Ensure that the Flask application code references the correct path to the trained model

7.2. Run the Flask application using the following command

```bash
flask run   
```

7.3. Open a web browser and go to http://localhost:5000 to access the locally hosted application.

    
## Usage
The application is designed to provide a straightforward experience for predicting cardiac conditions, specifically ST-segment elevation myocardial infarction (STEMI), from uploaded medical images. Follow these simple steps to use the application:

1. Access the Application:

1.1. Ensure that the Flask application is running locally by executing the command

```bash
flask run 
```

1.2. Open your web browser and go to http://localhost:5000


2. Image Upload:

2.1. On the application's interface, locate the option to upload medical images

2.2. Click the designated area or button to select and upload the image you want to analyze


3. Prediction Report:

3.1. Once the image is uploaded, the AI assistant (DeepSTEMI) will process the data using the trained ResNet50 model

3.2. The application will generate a prediction report that includes:

•	The prediction result (STEMI or normal case)

•	Medical measures recommended based on the prediction

•	Date and time of the analysis

•	Other relevant information related to the prediction.

4. Review the Results

4.1. Examine the prediction report to understand the AI's assessment of the uploaded medical image.

4.2. Take note of the recommended medical measures provided in the report.

5. Repeat as Needed
5.1. You can upload multiple images for analysis.

5.2. Repeat the process for each image you want to assess.



## Important Notes for Contribution

Contributions are always welcome!

1. Interpretation of Results:

1.1. Understand that the prediction is based on the AI model's analysis of the provided medical images. Consult with healthcare professionals for comprehensive medical advice.

2. Feedback and Improvement:
2.1. Provide feedback on the application's predictions to contribute to continuous model refinement.

2.2. Consider collaborating with healthcare professionals to enhance the accuracy and reliability of the diagnostic system.


## License & Author Contribution

[MIT](https://choosealicense.com/licenses/mit/)

MIT License

Copyright (c) [2023] [Abdulazeez Albarade, Faris Alhuthali, Rafeef Elberim, Loay Albaradei, Ahmad Alhazmi, Somayah Albaradei]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
