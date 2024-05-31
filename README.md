<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sleep Health and Lifestyle Analysis</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background: #4CAF50;
            color: #fff;
            padding: 1rem 0;
            text-align: center;
            border-bottom: 2px solid #388E3C;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }

        header h2 {
            margin: 0;
            font-size: 1.5rem;
        }

        main {
            padding: 20px;
            max-width: 800px;
            margin: 20px auto;
            background: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        section {
            margin-bottom: 20px;
        }

        section h2 {
            border-bottom: 2px solid #4CAF50;
            padding-bottom: 5px;
        }

        section h3 {
            margin-top: 20px;
            margin-bottom: 10px;
        }

        ul {
            list-style-type: disc;
            margin-left: 20px;
        }

        code {
            background: #f4f4f4;
            padding: 2px 4px;
            border-radius: 4px;
        }
    </style>
</head>

<body>
    <header>
        <h1>Sleep Health and Lifestyle Analysis</h1>
        <h2>Maxyne Nuela Ignacio</h2>
    </header>

    <main>
        <section>
            <h2>I. Project Overview</h2>
            <p>Sleep is one of the significant maintainable components in a person’s overall health and well-being. It supports the immune system enabling the body to fight off various diseases, thus obtaining a quality sleep enhances the body function, memory, and reduces negative mental health factors such as anxiety, stress, and depression. Prioritizing good sleep health, maintaining a consistent sleep schedule, and creating a restful environment is vital in keeping a good health and well-being.</p>
            <p>Therefore, the analysis aims to analyze key user attributes such as Person ID, Gender, Age, Occupation, Sleep Duration, Quality of Sleep, Physical Activity Level, Stress Level, BMI Category, Blood Pressure, Heart Rate, Daily Steps, and Sleeping Disorder, using these data points to extract insights into data analysis and behavior. Through analyzing behavior and characteristics of the attributes, it will identify opportunities to enhance different businesses that cater to sleep lifestyle and elevate understanding more in individual experiences in relation to the topic.</p>
        </section>

        <section>
            <h3>The analysis of Sleep Health and Lifestyle Data utilizes several attributes to uncover patterns and preferences among the user base:</h3>
            <ul>
                <li><strong>Gender:</strong> Gender Analysis can reveal sleep patterns and health outcomes between males and females which increases the reader’s knowledge.</li>
                <li><strong>Age:</strong> The dataset for age can aid to predict appropriate recommendations and interventions for better sleep health.</li>
                <li><strong>Occupation:</strong> Understanding the line of work of every individual can further help the system to identify comparisons with workers who might have different sleep issues of shift or office workers.</li>
                <li><strong>Sleep Duration:</strong> Measuring sleep duration helps in understanding how much sleep individuals are getting and identifying those who are sleep-deprived.</li>
                <li><strong>Quality of Sleep:</strong> Evaluating the dataset and contrasting the quality of sleep based on gender, age, and occupation can furthermore identify its impact on physical and mental health.</li>
                <li><strong>Physical Activity:</strong> Physical activity levels can influence sleep patterns, and understanding this relationship can help promote better sleep through exercise.</li>
                <li><strong>Stress Level:</strong> Stress level analysis can show how stress impacts sleep quality and duration, providing insights for stress management interventions.</li>
                <li><strong>Body Mass Index (BMI) Category:</strong> BMI data can help assess the relationship between body weight and sleep disorders, informing weight management strategies for better sleep.</li>
                <li><strong>Blood Pressure:</strong> Monitoring blood pressure in relation to sleep can identify risks associated with poor sleep patterns.</li>
                <li><strong>Heart Rate:</strong> Heart rate analysis can indicate how sleep affects health and recovery.</li>
                <li><strong>Daily Steps:</strong> Tracking daily steps provides a measure of physical activity and its correlation with sleep quality.</li>
                <li><strong>Sleeping Disorder:</strong> Identifying sleep disorders is crucial for diagnosing and treating specific sleep-related health issues.</li>
            </ul>
        </section>

        <section>
            <h2>II. Libraries and Data Handling</h2>
            <h3>Libraries Used</h3>
            <p>List and describe the libraries used in the project for data manipulation and visualization, e.g., Pandas, Matplotlib, Seaborn.</p>
            <ul>
                <li><strong>Pandas:</strong> Pandas is an open-source Python package that is most widely used for data science/data analysis and machine learning tasks. It is built on top of another package named Numpy, which provides support for multi-dimensional arrays. As one of the most popular data wrangling packages, Pandas works well with many other data science modules inside the Python ecosystem, and is typically included in every Python distribution.
                    <pre><code>import pandas as pd</code></pre>
                </li>
                <li><strong>OS:</strong> The OS module in Python provides functions for interacting with the operating system. OS comes under Python's standard utility modules. This module provides a portable way of using operating system-dependent functionality.
                    <pre><code>import os</code></pre>
                </li>
                <li><strong>Warnings:</strong> The warnings module in Python provides a way to control how warnings are handled within a Python script. It allows developers to emit warning messages to alert users of potential issues or unexpected behavior in their code.
                    <pre><code>import warnings
warnings.filterwarnings('ignore')</code></pre>
                </li>
                <li><strong>NumPy:</strong> NumPy is a Python library used for working with arrays. It also has functions for working in the domain of linear algebra, Fourier transform, and matrices. NumPy was created in 2005 by Travis Oliphant. It is an open-source project and you can use it freely.
                    <pre><code>import numpy as np</code></pre>
                </li>
                <li><strong>SciPy:</strong> SciPy is a scientific computation library that uses NumPy underneath. SciPy stands for Scientific Python. It provides more utility functions for optimization, stats and signal processing. Like NumPy, SciPy is open source so we can use it freely.
                    <pre><code>from scipy import stats</code></pre>
                </li>
                <li><strong>Seaborn:</strong> Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics. Seaborn helps you explore and understand your data.
                    <pre><code>import seaborn as sns</code></pre>
                </li>
                <li><strong>Plotly Express:</strong> Plotly express is a high-level data visualization package that allows you to create interactive plots with very little code. It is built on top of Plotly Graph Objects, which provides a lower-level interface for developing custom visualizations.
                    <pre><code>import plotly.express as px
import plotly.graph_objects as go
import plotly.figure_factory as ff</code></pre>
                </li>
                <li><strong>Termcolor:</strong> Termcolor is a Python module for printing colored text in the terminal. It allows you to add color and styling to text output, making it easier to distinguish between different types of information or highlight important messages.
                    <pre><code>from termcolor import colored</code></pre>
                </li>
                <li><strong>Matplotlib:</strong> Matplotlib is a powerful and very popular data visualization library in Python. In this tutorial, we will discuss how to create line plots, bar plots, and scatter plots in Matplotlib using stock market data in 2022.
                    <pre><code>import matplotlib.pyplot as plt
import matplotlib.colors as mcolors</code></pre>
                </li>
                <li><strong>Imbalanced-learn (imblearn):</strong> imbalanced-learn is an open-source python toolbox aiming at providing a wide range of methods to cope with the problem of imbalanced dataset frequently encountered in machine learning and pattern recognition.
                    <pre><code>from imblearn.over_sampling import SMOTE</code></pre>
                </li>
                <li><strong>Scikit:</strong> Scikit-learn is probably the most useful library for machine learning in Python. The sklearn library contains a lot of efficient tools for machine learning and statistical modeling including classification, regression, clustering, and dimensionality reduction.
                    <pre><code>from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import classification_report</code></pre>
                </li>
            </ul>
        </section>

        <section>
            <h2>III. Data Analysis and Findings</h2>
            <p>Describe the steps taken to analyze the data, including any preprocessing, feature selection, and modeling techniques used.</p>
            <p>Summarize the key findings and insights obtained from the analysis.</p>
        </section>

        <section>
            <h2>IV. Conclusion</h2>
            <p>Summarize the overall findings and implications of the project. Discuss any limitations and potential future work.</p>
        </section>
    </main>
</body>

</html>

