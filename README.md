# Discord User Info API

This Node.js application serves as a simple API for retrieving extended information about Discord users. It utilizes the Discord API to fetch user data and processes it to provide additional details. The API exposes an endpoint to retrieve user information based on their Discord user ID.

## How to Run

Follow these steps to run the application locally:

1. Clone the repository to your local machine.

    ```bash
    git clone https://github.com/itsvijaysingh/Discord-Lookup-API.git
    ```

2. Navigate to the project directory.

    ```bash
    cd Discord-Lookup-API
    ```

3. Install the required dependencies.

    ```bash
    npm install
    ```

4. Open the `api.js` file and ensure the `DISCORD_BOT_TOKEN` variable is set. You can obtain a Discord bot token by creating a new bot on the [Discord Developer Portal](https://discord.com/developers/applications).

    ```javascript
    const DISCORD_BOT_TOKEN = process.env.DISCORD_BOT_TOKEN || 'your-bot-token-here';
    ```

5. Save the changes.

6. Run the application.

    ```bash
    node api.js
    ```

7. The server will start running on `http://localhost:3000`. You can now make requests to the API.

## API Endpoint

- **GET /api/user/:id**: Retrieve extended information about a Discord user based on their user ID.

    Example: `http://localhost:3000/api/user/123456789012345678`

    Replace `123456789012345678` with the actual Discord user ID.

    The response will include details such as username, discriminator, avatar, banner, user flags, Nitro type, creation date, and more.

## Dependencies

- [Express](https://expressjs.com/): A web application framework for Node.js.
- [Cors](https://www.npmjs.com/package/cors): Middleware for enabling Cross-Origin Resource Sharing.

**Note:** Ensure that Node.js is installed on your machine before running the application.

Feel free to customize and extend the application according to your needs. If you encounter any issues or have questions, please refer to the [Discord API documentation](https://discord.com/developers/docs/intro) for assistance.
