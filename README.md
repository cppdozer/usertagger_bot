Telegram User Tagger
====================

This code provides a Telegram bot that can be used to tag and message users in a Telegram chat. It utilizes the `telegram` and `telethon` libraries to interact with the Telegram API.

Prerequisites
-------------

Before running the code, make sure you have the following prerequisites:

-   Python 3.x
-   `telegram` library (install with `pip install python-telegram-bot`)
-   `telethon` library (install with `pip install telethon`)

Getting Started
---------------

1.  Clone the repository or copy the code into your local development environment.
2.  Install the required libraries mentioned in the Prerequisites section.
3.  Obtain a Telegram Bot API token from [BotFather](https://core.telegram.org/bots#botfather) and replace the `Token` variable in the code with your token.
4.  Set the `accountID` and `accountHash` variables with your Telegram account ID and hash.
5.  Customize the logging settings if needed.
6.  Run the code.

Usage
-----

The bot listens for the `/utag` command in a Telegram chat. Only administrators or the creator of the chat can use this command.

### Command Syntax

bashCopy code

`/utag [message]`

-   `message` (optional): The message you want to send to the tagged users.

### Examples

1.  Tag all members without sending a message:

    bashCopy code

    `/utag`

2.  Tag all members and send a message:

    bashCopy code

    `/utag Hello everyone!`

Functionality
-------------

When the `/utag` command is received, the bot retrieves the list of chat members and removes any bot accounts. It then splits the member list into subarrays and sends messages containing the tagged members.

The bot pauses for 3.5 seconds between each message to avoid rate limits imposed by the Telegram API.

Logging
-------

The code includes a basic logging configuration to log messages at the INFO level. You can modify the logging format or level according to your needs.

Contributions
-------------

Contributions to the code are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

License
-------

This code is licensed under the [MIT License](https://opensource.org/licenses/MIT). Feel free to use, modify, and distribute it as per the terms of the license.
<br>
Coded by **[cppdozer](https://github.com/cppdozer)**
