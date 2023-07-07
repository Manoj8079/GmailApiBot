# mailBot-NodeJs

This is a Node.js application that automatically sends an auto-reply to unread emails in Gmail using the Gmail API. The application runs as a server and periodically checks for unread messages in the user's inbox. If an unread message is found, it sends an auto-reply and moves the original message to a labeled folder called "AutoReplied".

## Prerequisites

Before running the application, make sure you have the following prerequisites:

- Node.js (version 12 or higher)
- Gmail API credentials (JSON file)

## Installation



1. Navigate to the project directory:

    ```
    cd gmail-auto-reply
    ```

2. Install dependencies using npm:

    ```
    npm install
    ```

3. Add your Gmail API credentials:

    - create the credentials.json file.
    - Replace path/to/your/credentials.json with the actual path to your Gmail API credentials JSON file.

## Usage

1. Start the application:

    ```
    npm start
    ```

2. The application will start a server on port 8080.

3. Open a web browser and go to http://localhost:8080 to initiate the auto-reply process.

4. The application will authenticate using the provided Gmail API credentials and periodically check for unread messages in the inbox.

5. If an unread message is found, the application will send an auto-reply email and move the original message to the "AutoReplied" labeled folder.

## Configuration

You can customize the behavior of the application by modifying the following variables in the `index.js` file:

    - `SCOPES`: An array of Gmail API scopes required for the application.
    - `labelName`: The name of the labeled folder where the original messages will be moved.
