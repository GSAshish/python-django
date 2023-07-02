
- git
- vscode
-  nglok => makes localhost url   https Testing by making a url for testing
-  postman
- 
1. **django-compressor**: It is a Django app that helps manage the versioning and packaging of CSS and JavaScript files. It allows you to write your stylesheets and JavaScript code in separate files and then automatically combines and minifies them for production. It also provides features like cache control and template tags for easy inclusion of compressed files in your templates.

In addition to the styling version manager tool, you will also need package manager tools to handle your Python dependencies and manage your project's packages. The commonly used package manager for Python is:

1. **pip**: Pip is the default package manager for Python, and it is used to install, upgrade, and manage Python packages. You can define your project's dependencies in a `requirements.txt` file and use pip to install them.

Apart from these tools, there are a few other considerations for production-level code in Django:

1. **Static file management**: Django provides a built-in mechanism to manage static files (CSS, JavaScript, images, etc.) in your project. You can define the location of your static files and serve them using Django's static file handling. In production, it's recommended to use a separate web server (such as Nginx or Apache) to serve static files for better performance.

2. **Deployment tools**: To deploy your Django project in a production environment, you'll need tools and frameworks that assist with the deployment process. Popular deployment tools for Django include Ansible, Fabric, and Docker. These tools help automate the deployment process, manage server configurations, and ensure a smooth deployment workflow.

3. **Error logging and monitoring**: It's crucial to have error logging and monitoring in place to track and handle any errors that occur in your Django application. Tools like Sentry and Rollbar provide error tracking and reporting, allowing you to identify and fix issues in a timely manner.

4. **Performance optimization**: For production-level code, it's essential to optimize the performance of your Django application. This can include techniques such as caching, database optimization, code profiling, and using tools like Django Debug Toolbar to identify performance bottlenecks.

PEP 8 is a style guide for Python code. It provides guidelines and recommendations for writing clean, readable, and consistent Python code. Following PEP 8 helps improve code quality, maintainability, and collaboration among developers. Here are some key points from PEP 8:

1. **Indentation**: Use 4 spaces for indentation. Do not use tabs.

2. **Line length**: Limit lines to a maximum of 79 characters. If a line needs to be longer, it should be broken into multiple lines using parentheses or backslashes.

3. **Import statements**: Each import statement should be on a separate line. Group imports into three sections: standard library imports, related third-party imports, and local application imports. Sort the imports alphabetically within each section.

4. **Whitespace**: Use a single space around operators and after commas. Avoid extraneous whitespace at the beginning or end of lines.

5. **Naming conventions**: Use lowercase letters and underscores for variable and function names. Use CapitalizedWords (also known as CamelCase) for class names. Use uppercase letters for constants.

6. **Function and method definitions**: Use a space between the function name and the opening parenthesis. Place any arguments or parameters inside the parentheses, separated by commas.

7. **Comments**: Use comments to explain complex code or provide additional context. Place comments on a separate line or use inline comments sparingly. Comments should be clear, concise, and relevant.

8. **Documentation strings (docstrings)**: Use docstrings to document modules, functions, classes, and methods. Docstrings should describe the purpose, behavior, and usage of the code element.

9. **Code layout**: Organize your code with logical structure and spacing. Use blank lines to separate logical sections of code.

These are just some of the guidelines provided by PEP 8. It is recommended to read the full PEP 8 document to understand all the details and conventions. There are also various tools available that can automatically check your code for PEP 8 compliance, such as `pycodestyle`, `flake8`, and integrated linters in code editors like PyCharm and Visual Studio Code.