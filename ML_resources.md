# Machine Learning Resources
This file contains a curated list of resources related to the machine learning aspect of the SnapScribe. These resources can be useful for understanding the techniques used in sequence modeling, computer vision, and image captioning.  
It also details the expected workflow when developing a real world ML project. PRs are expected to follow the workflow and participants will be required to understand (atleast some, because its definitely not a good idea to dive into a rabbit hole of studying and never applying) aspects.

## Online Courses, Resources, YT Playlists
[MIT 6.S191 Introduction to Deep Learning](https://youtube.com/playlist?list=PLtBw6njQRU-rwp5__7C0oIVt26ZgjG9NI) - Great introduction to Neural Networks, CNNs, RNNs, LSTMs, Transformer models. Watch only the 2023 videos. Recommended to get started as this will get you up and running the fastest. Only the first 3 videos are really necessary.

[Coursera - Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction) - Basic intro to ML topics including stuff like Linear Regression, Logistic Regression etc. The first course in this specialization won't be of much direct use to this project but it is still recommended to complete it. The second course has intro to Neural Networks and CNNs which is relevant to this project.

[Coursera - Deep Learning Specialization](https://www.coursera.org/specializations/deep-learning) - A comprehensive specialization covering various topics in deep learning, including convolutional neural networks (CNNs), recurrent neural networks (RNNs), and sequence modeling.

[Fast.ai - Practical Deep Learning for Coders](https://www.fast.ai/) - A practical course that teaches deep learning by building real-world applications. It provides hands-on experience with state-of-the-art techniques.

[Learn PyTorch](https://www.learnpytorch.io/) - An excellent resource to give you a flavour of the complete life-cycle of an ML Project, paper-replication and model deployment. Also, go through all the extra resources if you can!

[PyTorch in 25hrs](https://www.youtube.com/watch?v=V_xro1bcAuA&t=523s&pp=ygUIcHl0b3JjaCA%3D) - Not meant to be finished in a day! Take your time.

## Research Papers (Optional) 
### [MIT 6.S191 is compulsory before going through this]
Something that you will often need to do while learning ML topics or implementing things, is reading research papers. So while this part of the project isn't mandatory considering the timeline, take a look at a bit of the following research paper (remember: you don't have to understand everything you read, trust me there will be a lot that you don't understand. Never hesitate to Google topics to try to learn more about them). 

**NOTE**: It is recommended to only try to read the below once you know the basics of Neural Networks, CNNs, RNNs, LSTMs, and have heard/watched something introductory about Transformer Attention Models. Remember not to dive too deep into the mathematics for every topic. You can just dip your toes and understand the basics and how to implement each using Tensorflow/PyTorch. The basics are all that is required.

[Show and Tell: A Neural Image Caption Generator](https://arxiv.org/pdf/1411.4555) - The original research paper by Vinyals et al. that introduces the concept of using neural networks for generating image captions.

[Bottom-Up and Top-Down Attention for Image Captioning and Visual Question Answering](https://arxiv.org/pdf/1707.07998) - A research paper by Anderson et al. that proposes an attention mechanism for image captioning, allowing the model to focus on relevant image regions.

## Blogs and Tutorials
[Machine Learning Mastery](https://machinelearningmastery.com/) - A blog by Jason Brownlee offering a wealth of tutorials, articles, and resources on various machine learning topics.

[Towards Data Science](https://towardsdatascience.com/) - An online platform featuring a wide range of data science and machine learning articles, tutorials, and case studies. You'll find many useful ML and data science blogs here along with follow-along tutorials and Github repos where you can get help from.

## Kaggle Project-Specific Resources
[Flickr8K Image Captioning using CNNs+LSTMs](https://www.kaggle.com/code/quadeer15sh/flickr8k-image-captioning-using-cnns-lstms) - This is a Kaggle notebook containing a specific implementation of image captioning. You can use this as a resource material. Your notebook must not be a copy of this. Even if drawing mostly from this, you will need to prove that you have experimented with various stuff and architectures in your notebook.

## Workflow of ML Project
The following is the general workflow of development of an ML project. It is not specific to this project, it just provides a general overview.  
**NOTE**: Some steps may/may not be relevant to this project.
### 1. Notebook Development:

- Data Loading and Exploration: Load the dataset into the notebook and perform initial exploratory data analysis (EDA). This includes understanding the data structure, visualizing distributions, handling missing values, and identifying potential preprocessing steps.
- Data Preprocessing: Clean the data by addressing missing values, handling outliers, performing feature scaling, and transforming categorical variables.
- Feature Engineering: Create new features or modify existing ones to improve model performance. This could involve dimensionality reduction techniques, creating interaction terms, or encoding categorical variables.
- Model Development: Train and evaluate different ML models using appropriate algorithms for the task at hand (e.g., classification, regression, or clustering). Use cross-validation techniques to assess model performance and hyperparameter tuning to optimize model accuracy.
- Model Evaluation: Assess model performance using suitable evaluation metrics, such as accuracy, precision, recall, F1 score, or mean squared error (MSE). Consider additional techniques like model interpretation and visualization to gain insights into model behavior.

### 2. Converting Notebook to a Python Script:
- Refactor Code: Organize the code into functions or classes to improve readability and maintainability. Remove any unnecessary or redundant code sections.
- Modularize Notebook Code: Split the notebook code into logical sections, such as data loading, preprocessing, model training, and evaluation.
- Define Input and Output: Determine how the Python script will receive input data and generate output results. This may involve defining command-line arguments or utilizing input/output files or directories.
- Export Dependencies: Identify and list the required dependencies and libraries used in the notebook. Make sure to include these dependencies in the Python script's environment.
- Create a Python Script: Copy and paste the relevant sections of code from the notebook (ipynb file) into a Python script file (e.g., script.py). Modify the code as necessary to account for changes in variable names, imports, or other specific requirements.
### 3. Deployment and Productionization:
- Test the Script: Validate the Python script by running it locally and comparing the results with those obtained in the notebook.
- Prepare Data: Ensure that the input data for the Python script follows the required format and preprocessing steps.
- Model Persistence: Save the trained ML model and any required preprocessing steps (e.g., encoders, scalers) to disk.
- Set up Environment: Install the necessary dependencies and libraries in the deployment environment.
- Automate Execution: Incorporate the Python script into an automated workflow, such as a batch job or web service, to handle data input, model prediction, and result output. You will have to set up routes in the backend Flask app for serving predictions (here, captions for image)
- Monitor Performance: Implement mechanisms to monitor the script's performance, detect errors or anomalies, and log relevant information during execution.
- Iterate and Update: Continuously update and improve the script based on feedback, new data, or model enhancements. Consider version control practices and documentation for reproducibility.

### Additional Functionality
Additionally, you can also test this web app with images generated by prompting DALL-E, OpenAI's generative image model and see how closely your caption matches your original prompt. But this should only be explored once the other parts of the project are functional.