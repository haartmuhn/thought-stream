<div align="center">

# Thought Stream

[![License: MIT](https://img.shields.io/badge/License-MIT-darkgreen.svg)](https://opensource.org/licenses/MIT)
![JavaScript Badge](https://img.shields.io/badge/js-F7DF1E?logo=javascript&logoColor=000&style=flat)
![JSON Badge](https://img.shields.io/badge/json-FF0000?logo=json&logoColor=fff&style=flat)
![npm Badge](https://img.shields.io/badge/npm-A020F0?logo=npm&logoColor=fff&style=flat)
![Node.JS Badge](https://img.shields.io/badge/node-orange?logo=node.js&logoColor=fff&style=flat)

</div>

## Description

Thought Stream is a social network API designed to allow users to share their thoughts, react to friends' thoughts, and manage their friend lists. Built using Express.js, MongoDB, and Mongoose, Thought Stream is a robust and scalable platform capable of handling large amounts of unstructured data.

## Table of Contents

- [Description](#description)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [Tests](#tests)
- [License](#license)

## Installation

1.  Clone the repository:

```bash
git clone https://github.com/haartmuhn/thought-stream.git
cd thought-stream
```

2.  Install the dependencies:

```
npm install
```

3.  Set Up Environmental Variables:

Create a `.env` file in the root directory and set your MongoDB URI and other configuration details:

```makefile
MONGODB_URI=your-mongodb-uri
```

4.  Start the Server:

 ```bash
npm start
 ```

Open your web browser and navigate to `http://localhost:3001` to view the application.

## Usage

Thought Stream provides a set of API endpoints for managing users, thoughts, reactions, and friends. You can test these endpoints using tools like Insomnia.

API Endpoints
-   Users:
    -   GET `/api/users`: Get all users
    -   GET `/api/users/:id`: Get a user by ID
    -   POST `/api/users`: Create a new user
    -   PUT `/api/users/:id`: Update a user by ID
    -   DELETE `/api/users/:id`: Delete a user by ID
-   Thoughts:
    -   GET `/api/thoughts`: Get all thoughts
    -   GET `/api/thoughts/:id`: Get a thought by ID
    -   POST `/api/thoughts`: Create a new thought
    -   PUT `/api/thoughts/:id`: Update a thought by ID
    -   DELETE `/api/thoughts/:id`: Delete a thought by ID
-   Reactions:
    -   POST `/api/thoughts/:thoughtId/reactions`: Create a reaction for a thought
    -   DELETE `/api/thoughts/:thoughtId/reactions/:reactionId`: Delete a reaction by ID
-   Friends:
    -   POST `/api/users/:userId/friends/:friendId`: Add a friend
    -   DELETE `/api/users/:userId/friends/:friendId`: Remove a friend

Thought Stream ensures smooth navigation through these options, guiding users at every step of the process. To gain a better understanding of how Thought Stream operates, below is a demonstration of the application's functionality:

<div align="center">

[thought-stream.webm](https://github.com/user-attachments/assets/8eaec549-ecdc-4159-adcc-f8585d54963b)

</div>

## Features

-   **User Management**: Create, read, update, and delete users, along with managing a friend list.
-   **Thought Sharing:** Users can post thoughts and update or delete them.
-   **Reactions**: Engage with others' thoughts by adding or removing reactions.
-   **Data Validation**: Ensures that user inputs are correctly formatted and validated.
-   **Flexible & Scalable**: Built with NoSQL, allowing for scalable data management.

## Contributing

Contributions to Thought Stream are welcome! Here’s how you can contribute:

1. **Fork the repository** on GitHub.
2. **Create a branch** for your feature `git checkout -b new-feature`.
3. **Make changes** and commit them `git commit -m "Add some feature"`.
4. **Push to the branch** `git push origin new-feature`.
5. **Create a new Pull Request** against the main.

Please ensure your code adheres to the existing style of the project to make your changes easy to understand and integrate!

## Tests

To run tests, execute the following command:

```
npm test
```

(Note: You will need to write the tests based on the endpoints and operations your application performs, as this is not set up by default.)

## License

Thought Stream is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute this application according to the terms of the license.
