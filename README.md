# Azure_Web_Apps_Flask

## Azure Python Web App

This is a simple Flask web application that demonstrates basic HTML, CSS, and JavaScript integration with Python. The app also includes smooth animations using the **GSAP** JavaScript library.

## Prerequisites

Before you begin, ensure you have the following installed:

- **Python 3.x**: Make sure you have Python 3 installed on your machine. You can check by running `python3 --version` in your terminal.
- **pip**: Python's package installer.

### Optional:
- **VSCode** (or your preferred code editor) with Python extension.

## Installation

1. **Clone the Repository**:

   If you haven't already, clone this repository to your local machine:

   ```bash
   git clone <your-repository-url>
   cd <your-repository-folder>
### Set Up Virtual Environment (recommended):
It's a good practice to use a virtual environment for Python projects. This ensures that your dependencies don't conflict with other projects.
 ```
  python3 -m venv venv
 
 source venv/bin/activate
``` 
# On macOS/Linux
If you're on Windows, use the following command to activate the environment:

```venv\Scripts\activate```
### Install Dependencies:
Install the necessary Python packages by running:

```pip install -r requirements.txt```
If you don't have a requirements.txt file yet, you can install Flask manually:

```pip install flask```
Create requirements.txt (if not already created):
If you need to create the requirements.txt file, you can do so by running:

  ```pip freeze > requirements.txt```

## Running the App Locally

To run the app locally, follow these steps:

Activate Your Virtual Environment (if not already activated):
  ```source venv/bin/activate ``` 
# On macOS/Linux
Run the Flask App:
  Start the Flask development server by running:

  ```python app.py```
  
By default, Flask will run the app on http://127.0.0.1:5000.

If you get a port conflict error, you can change the port number in app.py:
```
   if __name__ == "__main__":
      app.run(debug=True, port=5001)
```
# Change port to 5001
Open the App in Your Browser:
Open your browser and visit http://127.0.0.1:5000 (or the port you've specified). You should see your web page running with animations!
Project Structure

app.py: The main Python file for the Flask app.

templates/: Directory for HTML templates.

index.html: The main webpage with some animations and UI.

static/: Directory for static files like CSS and JavaScript.

styles.css: The CSS file for styling the page.

requirements.txt: A file listing all Python dependencies (if applicable).

### Features

Flask as the backend web framework.
GSAP (GreenSock Animation Platform) used to create smooth animations.
Responsive design with simple CSS styling.
Troubleshooting

### Port Conflict Error:
  If you get an error that says "Address already in use," it means another application is using port 5000. You can either kill the process using the port or change the port number in app.py.
### Missing Flask Module:
  If you see an error like ModuleNotFoundError: No module named 'flask', make sure you have installed Flask by running:
     ``` pip install flask ```
  
### Deployment

## To deploy the app on Azure Web Apps:

Create an Azure Web App from the Azure Portal.

Set up GitHub integration to deploy directly from your repository.

Push your code to GitHub.

In the Azure Deployment Center, link your repository and choose the branch to deploy.

Azure will automatically deploy your Flask app to the cloud.

### License

This project is licensed under the MIT License - see the LICENSE file for details.


---

This README is now formatted correctly for GitHub. You can copy-paste it directly into a `README.md` file in your project repository.

Let me know if you need any further changes!
