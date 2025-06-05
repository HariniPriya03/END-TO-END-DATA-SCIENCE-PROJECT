# END-TO-END-DATA-SCIENCE-PROJECT
Student Score Predictor Web App
What’s This Project About?
This is a simple web app that predicts how well a student might score on an exam based on how many hours they studied. You start by training a straightforward machine learning model on some sample data — hours studied vs. scores achieved — and then you build a web app so anyone can enter study hours and instantly see their predicted score.

It’s like a mini end-to-end project that covers everything from data and model training to making it easy to use through a website.

How Did I Build It?
Training the Model:
I used Python’s pandas library to load the data from a CSV file, then trained a Linear Regression model with scikit-learn. Once the model learned the relationship between hours studied and scores, I saved it as a file (model.pkl) using joblib. This step just needs to be done once — unless you want to train on new data.

Making the Web App:
Using Flask, a lightweight web framework in Python, I created a small website with an input form. You enter the number of hours you studied, submit it, and the app runs the saved model to predict your score. The result is then shown right on the page.

Putting It All Together:
The training script and the web app script live in the same folder. The web app uses the saved model, so it’s fast and doesn’t have to retrain every time you visit the page.

How to Run It on Your Computer
Open the project folder in VSCode (or any code editor).

Set up a Python virtual environment (to keep things organized).

Install the needed Python packages: pandas, scikit-learn, flask, and joblib.

Run the training script to create the model file.

Then run the Flask app.

Open your browser to http://127.0.0.1:5000 and try it out!

What Does the Web App Look Like?
It’s super simple: a clean webpage with a box where you type in how many hours you studied. When you hit submit, it shows you the predicted score right below.

No fancy graphics — just pure functionality focused on showing how a machine learning model can interact with users through a website.

Why Is This Useful?
It’s a great way to learn how to go from raw data to a usable web app.

Shows how machine learning models can be integrated into web applications.

Useful if you want to quickly share predictions without complex setups.

Can be the base for more advanced projects — like adding more features, better data, or nicer UI.

What Should You Keep in Mind?
Your model is only as good as the data — this one is just an example.

The index.html file (the webpage) must be inside a folder called templates — Flask looks there for HTML files.

Always run the training script first, so your model file exists before starting the web app.

Make sure you’re running commands inside the right folder where your code lives.

How Can You Improve This?
Add checks to make sure the input hours are valid numbers.

Make the website look nicer with some CSS styling.

Add more data or different features for better predictions.

Deploy the app online so friends can use it anywhere.

Extend it into a full student dashboard with more analytics.

In a Nutshell
You now have a working web app that uses a machine learning model behind the scenes to predict exam scores based on study hours. It’s a hands-on project that takes you through data handling, training a model, saving it, and creating a user-friendly interface to access it.

It’s simple, educational, and a solid base if you want to build more complex apps later on!
