# Chapter 23 Final: Build a Project with Integrating Tools

## Learn Python fast with some content ideas

Learning Python is a great choice, especially given your interest in web development, mobile app development, and software engineering. Here are some excellent resources to get you started:

**1. LearnPython.org:** This interactive Python tutorial offers free lessons for beginners. It covers topics like variables, loops, functions, and more. You can even get certified after completing the [`tutorials[1]`](https://www.learnpython.org/).

**2. Python Official Documentation:** The official Python documentation provides comprehensive information about the language. Start with the Python Tutorial for beginners and explore further as you gain [`confidence[2]`](https://stackoverflow.com/questions/70577/best-online-resource-to-learn-python).

**3. freeCodeCamp’s Python Courses:**
**- [`Full Course for Beginners`](https://www.freecodecamp.org/news/learn-python-free-python-courses-for-beginners/):** This YouTube course covers programming basics, including lists, conditionals, strings, and small projects like a calculator and a guessing game.
**- [`The Ultimate Python Beginner’s Handbook`](https://www.freecodecamp.org/news/the-python-guide-for-beginners/)** Dive deeper into Python concepts and explore its growing popularity [`3`](https://www.freecodecamp.org/news/learn-python-free-python-courses-for-beginners/) and [`4`](https://www.freecodecamp.org/news/the-python-guide-for-beginners/).

**REMEMBER:** practice coding regularly, work on small projects, and explore real-world examples.

## What is Virtual Environments in Python?

A virtual environment in Python is an isolated environment that allows you to manage dependencies for a specific project without affecting other projects or the global Python installation. It ensures that each project can have its own dependencies, regardless of what dependencies every other project has.

### Key Benefits:

1. **Dependency Management**: Different projects can have different versions of the same package without conflict.
2. **Isolation**: Keeps your global Python environment clean and free from project-specific dependencies.
3. **Reproducibility**: Makes it easier to reproduce the environment on different machines, ensuring consistency.

### How to Create and Activate a Virtual Environment:

1. **Create a Virtual Environment**:

   ```sh
   python -m venv .venv
   ```

   This creates a virtual environment in a directory named [`.venv`].

2. **Activate the Virtual Environment**:

   - On Windows:
     ```sh
     .venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```sh
     source .venv/bin/activate
     ```

3. **Deactivate the Virtual Environment**:
   ```sh
   deactivate
   ```

### Example:

```sh
# Create a virtual environment
python -m venv .venv

# Activate the virtual environment
.venv\Scripts\activate  # On Windows
# source .venv/bin/activate  # On macOS/Linux

# Install packages
pip install requests

# Deactivate the virtual environment
deactivate
```

Using virtual environments is a best practice for Python development, ensuring that your projects remain clean, isolated, and manageable.

## Create Virtual Environment

py -m venv .venv
source .venv/Scripts/activate
py -m pip show requests
py -m pip install -U pip
python.exe -m pip install --upgrade pip
py -m pip install python-dotenv
py -m pip freeze > requirements.txt

https://home.openweathermap.org/api_keys
login into your account
copy API_KEY
Then, go to API
Then, see Current Weather Data
click on API doc button
API Call
https://api.openweathermap.org/data/2.5/weather?lat={lat}&lon={lon}&appid={API key}
Then, on the right hand side, click on Units of measurement

pypi.org

To activate a virtual environment in Python on a Windows machine, you can use the following command in your terminal:

```sh
.venv\Scripts\activate
```

If you are using PowerShell, the command would be:

```sh
.venv\Scripts\Activate.ps1
```

Make sure to replace [`.venv`] with the name of your virtual environment directory if it is different.

## How can I create a class in Python?

To run the provided Python code, follow these steps:

1. **Ensure you have the required packages installed**:
   Open a terminal and run:

   ```sh
   pip install requests python-dotenv
   ```

2. **Create a `.env` file**:
   In the same directory as your `weather.py` file, create a `.env` file and add your OpenWeatherMap API key:

   ```
   API_KEY=your_openweathermap_api_key
   ```

3. **Run the script**:
   In the terminal, navigate to the directory containing your [`weather.py`] file and run:
   ```sh
   python weather.py
   ```

This will execute the script, prompt you to enter a city name, and then display the current weather conditions for that city.

## Create a Final Project

First, go to web url: https://flask.palletsprojects.com/en/3.0.x/#user-s-guide
or you can search in google.com with flask pallets projects, then you will see Welcome to Flask — Flask Documentation (3.0.x)
after that click on the link: [`Flask | The Pallets Projects` ](https://palletsprojects.com/p/flask/) or (https://palletsprojects.com/)

To fix the import error, you need to make sure that the `waitress` package is installed in your Python environment.

```bash

pip install waitress

```

After running this command, the `waitress` package should be installed and the import error should be resolved.

It looks like the [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fchien%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Fwaitress%2Fwaitress%2F__init__.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Users/chien/.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/waitress/waitress/__init__.pyi') package is already installed in your environment. The issue might be with how it's being imported or used in your code.

Ensure that you are importing [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fchien%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Fwaitress%2Fwaitress%2F__init__.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Users/chien/.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/waitress/waitress/__init__.pyi') correctly in your [`server.py`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fd%3A%2FlearnPython%2FLesson23%2Fserver.py%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%5D 'd:\\learnPython\Lesson23\server.py') file. Here is an example of how to import and use [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fchien%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Fwaitress%2Fwaitress%2F__init__.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Users/chien/.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/waitress/waitress/__init__.pyi'):

```python
from waitress import serve
from myapp import app  # Assuming you have a Flask app in myapp.py

if __name__ == "__main__":
    serve(app, host='0.0.0.0', port=8080)
```

Make sure the import statement matches the correct usage of the `waitress` package. If the issue persists, try restarting your IDE or Python environment to ensure it recognizes the installed packages.

To ensure that the [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fchien%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Fwaitress%2Fwaitress%2F__init__.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Users/chien/.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/waitress/waitress/__init__.pyi') package is installed globally, you can use the following command:

```bash
py -m pip install waitress
```

This will install `waitress` in the global Python environment. After running this command, the import error should be resolved. If you still encounter issues, make sure your IDE is using the correct Python interpreter where `waitress` is installed.

The error message "Import 'waitress' could not be resolved from source" typically indicates that the [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fchien%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Fwaitress%2Fwaitress%2F__init__.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Users/chien/.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/waitress/waitress/__init__.pyi') package is not installed in your Python environment. To resolve this, you need to install the [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fchien%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Fwaitress%2Fwaitress%2F__init__.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Users/chien/.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/waitress/waitress/__init__.pyi') package using `pip`.

Here are the steps to install [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fchien%2F.vscode%2Fextensions%2Fms-python.vscode-pylance-2024.7.1%2Fdist%2Ftypeshed-fallback%2Fstubs%2Fwaitress%2Fwaitress%2F__init__.pyi%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Users/chien/.vscode/extensions/ms-python.vscode-pylance-2024.7.1/dist/typeshed-fallback/stubs/waitress/waitress/__init__.pyi'):

1. **Open the Integrated Terminal in Visual Studio Code:**

   - You can open the terminal by selecting `View > Terminal` from the menu or by using the shortcut `` Ctrl+`  ``.

2. **Install the `waitress` package:**

   - Run the following command in the terminal:
     ```sh
     pip install waitress
     ```

3. **Verify the Installation:**

   - After the installation completes, you can verify it by running:
     ```sh
     pip show waitress
     ```
   - This command should display information about the `waitress` package, confirming that it is installed.

4. **Restart Visual Studio Code:**
   - Sometimes, the IDE needs to be restarted to recognize newly installed packages.

After following these steps, the import error should be resolved. If you still encounter issues, ensure that your Python interpreter is correctly set in Visual Studio Code to the environment where `waitress` is installed.

Here's a quick reminder of what the `waitress` package does in your code:

- `waitress` is a production-quality pure-Python WSGI server. In your script, it is used to serve your Flask application on `host="0.0.0.0"` and `port=8000`.

If you have any further questions or run into other issues, feel free to ask!

The [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FPython312%2FLib%2Fsite-packages%2Fwaitress%2F__init__.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Python312/Lib/site-packages/waitress/__init__.py') package is installed correctly, as indicated by the output of [`pip show waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FPython312%2FLib%2Fsite-packages%2Fwaitress%2F__init__.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Python312/Lib/site-packages/waitress/__init__.py'). The issue might be related to the Python interpreter settings in Visual Studio Code.

Here are the steps to ensure that Visual Studio Code is using the correct Python interpreter:

1. **Open the Command Palette:**

   - You can open the Command Palette by pressing `Ctrl+Shift+P`.

2. **Select Python Interpreter:**

   - Type `Python: Select Interpreter` and select it from the dropdown.

3. **Choose the Correct Interpreter:**

   - From the list of available interpreters, select the one that corresponds to `C:\Python312\python.exe` (or the one where [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FPython312%2FLib%2Fsite-packages%2Fwaitress%2F__init__.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Python312/Lib/site-packages/waitress/__init__.py') is installed).

4. **Reload the Window:**
   - Sometimes, you may need to reload the window for the changes to take effect. You can do this by typing `Reload Window` in the Command Palette and selecting it.

After ensuring that the correct interpreter is selected, the import error should be resolved. If the issue persists, try restarting Visual Studio Code.

If you have any further questions or run into other issues, feel free to ask!

To run the server with the provided code, follow these steps:

1. **Ensure Dependencies are Installed:**

   - Make sure you have [`Flask`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FPython312%2FLib%2Fsite-packages%2Fflask%2Fapp.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A78%2C%22character%22%3A6%7D%5D 'c:/Python312/Lib/site-packages/flask/app.py') and [`waitress`](command:_github.copilot.openSymbolFromReferences?%5B%7B%22%24mid%22%3A1%2C%22path%22%3A%22%2Fc%3A%2FPython312%2FLib%2Fsite-packages%2Fwaitress%2F__init__.py%22%2C%22scheme%22%3A%22file%22%7D%2C%7B%22line%22%3A0%2C%22character%22%3A0%7D%5D 'c:/Python312/Lib/site-packages/waitress/__init__.py') installed. You can install them using `pip` if they are not already installed:
     ```sh
     pip install flask waitress
     ```

2. **Save the Code to a File:**

   - Save the provided code to a file named `server.py`.

3. **Run the Server:**

   - Open a terminal in the directory where `server.py` is located.
   - Run the server using the following command:
     ```sh
     python server.py
     ```

4. **Access the Server:**
   - Open a web browser and navigate to `http://localhost:8000` to access the server.

Here is the complete code for reference:

```python
from flask import Flask, render_template, request
from weather import get_current_weather
from waitress import serve

app = Flask(__name__)

@app.route('/')
@app.route('/index')
def index():
    return render_template('index.html')

@app.route('/weather')
def get_weather():
    city = request.args.get('city')

    # Check for empty strings or string with only spaces
    if not bool(city.strip()):
        # You could render "City Not Found" instead like we do below
        city = "Kansas City"

    weather_data = get_current_weather(city)

    # City is not found by API
    if not weather_data['cod'] == 200:
        return render_template('city-not-found.html')

    return render_template(
        "weather.html",
        title=weather_data["name"],
        status=weather_data["weather"][0]["description"].capitalize(),
        temp=f"{weather_data['main']['temp']:.1f}",
        feels_like=f"{weather_data['main']['feels_like']:.1f}"
    )

if __name__ == "__main__":
    serve(app, host="0.0.0.0", port=8000)
```

After running the server, you should be able to see the application running and handle requests as defined in your routes.

## Install TailwindCss

To install and use Tailwind CSS in a Python project, you typically need to set up a frontend build process. Here’s a step-by-step guide to integrate Tailwind CSS into your Python project:

1. **Install Node.js and npm:**

   - Tailwind CSS requires Node.js and npm. You can download and install them from [nodejs.org](https://nodejs.org/).

2. **Initialize npm in Your Project:**

   - Open a terminal in your project directory and run:
     ```sh
     npm init -y
     ```

3. **Install Tailwind CSS:**

   - Run the following command to install Tailwind CSS and its dependencies:
     ```sh
     npm install tailwindcss postcss autoprefixer
     ```

4. **Create Tailwind Configuration File:**

   - Generate a `tailwind.config.js` file by running:
     ```sh
     npx tailwindcss init
     ```

5. **Set Up PostCSS:**

   - Create a `postcss.config.js` file in your project root with the following content:
     ```js
     module.exports = {
       plugins: {
         tailwindcss: {},
         autoprefixer: {},
       },
     };
     ```

6. **Create Tailwind CSS Input File:**

   - Create a CSS file (e.g., `src/styles/tailwind.css`) and add the following lines:
     ```css
     @tailwind base;
     @tailwind components;
     @tailwind utilities;
     ```

7. **Build Tailwind CSS:**

   - Add a build script to your `package.json`:
     ```json
     "scripts": {
       "build:css": "npx tailwindcss -i ./src/styles/tailwind.css -o ./static/css/tailwind.css --minify"
     }
     ```
   - Run the build script:
     ```sh
     npm run build:css
     ```

8. **Include Tailwind CSS in Your HTML:**
   - Link the generated CSS file (`./static/css/tailwind.css`) in your HTML templates. For example, in a Flask template:
     ```html
     <!DOCTYPE html>
     <html lang="en">
       <head>
         <meta charset="UTF-8" />
         <meta
           name="viewport"
           content="width=device-width, initial-scale=1.0"
         />
         <link
           href="{{ url_for('static', filename='css/tailwind.css') }}"
           rel="stylesheet"
         />
         <title>Document</title>
       </head>
       <body>
         <h1 class="text-3xl font-bold underline">Hello, Tailwind CSS!</h1>
       </body>
     </html>
     ```

By following these steps, you will have Tailwind CSS integrated into your Python project, allowing you to use its utility classes in your HTML templates.

### Conclusion

In this chapter, we have successfully integrated various tools and technologies to build a comprehensive Python project. Here are the key takeaways:

1. **Learning Resources**: We explored several resources to learn Python quickly and effectively, including interactive tutorials, official documentation, and freeCodeCamp courses.

2. **Virtual Environments**: We learned the importance of virtual environments in Python for managing dependencies, ensuring isolation, and maintaining reproducibility across different projects.

3. **Weather Application**: We built a weather application using Flask, a popular web framework in Python. The application fetches current weather data from the OpenWeatherMap API and displays it to the user.

4. **Production Server**: We used `waitress`, a production-quality WSGI server, to serve our Flask application, ensuring it is ready for deployment.

5. **Tailwind CSS Integration**: We integrated Tailwind CSS into our project to enhance the frontend design. This involved setting up a frontend build process using Node.js, npm, and PostCSS.

By following these steps, you have gained practical experience in building and deploying a Python web application with a modern frontend framework. Keep practicing and exploring new tools and technologies to further enhance your skills.

