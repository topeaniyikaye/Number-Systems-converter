# Number-Systems-converter
# Number-Systems-converter

Number Systems Converter
Project Description
The Number Systems Converter is a web application that helps change numbers from one base to another. It supports conversions between binary, octal, decimal, and hexadecimal number systems.

Dependencies
To run this project, you will need:

Node.js
MongoDB Atlas
Express.js

1. Installation

    1. Clone the repository:

        git clone <repository-url>
        cd number-systems-converter


    2. Install the dependencies:
        npm install

    3. Set up MongoDB Atlas:

            Create an account on MongoDB Atlas.

            Create a new cluster and get the connection string.

            Replace the MongoDB URI in db.js with your connection string:

        e.g
        const mongoURI = 'your-mongodb-uri-here';
        mongoose.connect(mongoURI)
            .then(() => console.log('Connected to MongoDB Atlas'))
            .catch(err => console.error('Failed to connect to MongoDB Atlas', err));

2. Running the Application

    1. Start the server:
    node index.js

    2. Open the application in your browser:

    Navigate to http://localhost:3002 to access the Number Systems Converter.

3. Project Structure

    number-systems-converter/
    ├── README.md
    ├── app.js
    ├── converter.js
    ├── db.js
    ├── history.js
    ├── index.html
    ├── index.js
    ├── package.json
    ├── package-lock.json
    ├── styles.css
    ├── node_modules/

    File Descriptions:

        1. index.html: The main HTML file for the web application.
        2. app.js: Contains the frontend JavaScript code for handling user interactions.
        4. index.js: The main server file for the Express.js application.
        5. converter.js: Contains functions for converting numbers between different bases.
        6. db.js: Handles the MongoDB connection.
        7. history.js: Defines the schema for storing conversion history in MongoDB.
        8. styles.css: Contains the styles for the web application.
        9. package.json: Lists the project dependencies and scripts.
        10. package-lock.json: Records the exact versions of dependencies installed.

4. Usage
    Convert Numbers:
    Enter the number to be converted, select the base of the number, and select the base to which you want to convert.
    Click the "Convert" button to see the result.
    View Conversion History:

    The conversion history is displayed below the conversion form.
