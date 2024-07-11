# Currency Converter Bot

A currency converter bot developed using Dialogflow and Flask, integrated with a currency converter API, and deployed on Telegram.

## Table of Contents
- [Description](#description)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Description
The Currency Converter Bot is designed to provide real-time currency conversion rates via a chat interface. The bot is built using Dialogflow for natural language understanding, Flask for backend development, and is integrated with a currency converter API. The bot is hosted using ngrok and deployed on Telegram for easy access.

## Technologies Used
- **Dialogflow**: For creating and managing conversation intents.
- **Flask**: For developing the backend web application.
- **Currency Converter API**: For fetching real-time currency conversion rates.
- **ngrok**: For exposing the local Flask application to the internet.
- **Telegram**: For deploying the chatbot.

## Installation
1. **Create a Dialogflow Account**: Set up your intents and entities in Dialogflow.
2. **Set Up Flask**:
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    pip install -r requirements.txt
    ```
3. **Integrate Currency Converter API**:
    - Search for a suitable currency converter API [here](https://www.currencyconverterapi.com/docs).
    - Obtain an API key from the service provider.
    - Configure the API key in your Flask application by updating the configuration file or environment variables.
    ```python
    API_KEY = 'your_api_key_here'
    ```
4. **Enable Fulfillment in Dialogflow**: Enable webhook fulfillment and provide the ngrok URL.
5. **Run Flask Application Locally**:
    ```bash
    python app.py
    ```
6. **Expose Localhost with ngrok**:
    ```bash
    ngrok http 5000
    ```
   Copy the generated ngrok URL and paste it in the Dialogflow fulfillment settings.

## Usage
1. **Interact with the Bot on Telegram**: 
    - Start a chat with your Telegram bot.
    - Ask for currency conversions, e.g., "Convert 100 USD to EUR".
2. **Dialogflow Intents**: The bot uses predefined intents to understand and process user queries.
3. **Webhook Fulfillment**: Dialogflow sends requests to the Flask backend via the ngrok URL, which processes the request and returns the conversion rate.

## Features
- Real-time currency conversion.
- Natural language understanding via Dialogflow.
- Integration with Telegram for easy access.
- Scalable backend using Flask.
- Secure and live hosting using ngrok.

## Contributing
If you would like to contribute to this project, please follow these guidelines:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
For any questions or support, please contact:
- **Pavankumar**: [pavankurapati0105@gmail.com]

---

Feel free to modify this template according to your specific requirements and additional details about your project.
