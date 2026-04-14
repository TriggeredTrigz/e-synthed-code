# e-synthed-code

## Overview
This tool is designed to simplify and automate tasks directly from the terminal. It provides a user-friendly interface and powerful features to enhance productivity and streamline workflows.

## Installation and usage
To use the tool, , follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/TriggeredTrigz/e-synthed-code.git
   ```
2. Navigate to the tool's directory:
   ```bash
   cd e-synthed-code
   ```
3. Create a virtual python environment and activate it:
   ```bash
   python -m venv .venv
   ```
   
   For Windows,
   ```bash
   .venv/Scripts/activate
   ```

   For Linux and Mac,
   ```bash
   source .venv/bin/activate
   ```
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Finally, run the following command:
   ```bash
   python app.py
   ```

This will display the app with all available options.

## Configuration
The tool requires a GROQ API key from their website in a .env file in the same directory. \
Example .env file is included. If using Docker Compose, the `GROQ_API_KEY` inside the `.env` file will automatically be passed into the container as an environment variable.

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-branch
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-branch
   ```
5. Open a pull request.

## Support
If you encounter any issues, feel free to open an issue in the repository or contact the maintainer.