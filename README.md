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

## Database (Optional)
By default, the application smoothly falls back to a local SQLite database (`local_fallback.db`) to store prompts when a PostgreSQL server isn't running. However, if you would prefer to use a PostgreSQL database, a separate Docker Compose file is provided to quickly spin one up:

```bash
docker compose -f docker-compose.postgres.yml up -d
```
This will natively start a PostgreSQL container on default port `5432` and initialize it so the Python app will seamlessly connect to it. 

It uses standard defaults (user: `postgres`, password: `postgres`, db: `postgres`). You can easily customize these defaults by filling out the `POSTGRES_` variables in your `.env` file (see `.env.example`). Ensure Docker is running before executing the command.

## Configuration
The tool requires a GROQ API key from their website in a .env file in the same directory. \
Example .env file is included.

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