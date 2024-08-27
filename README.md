# Request Header Parser Microservice

This is the Request Header Parser Microservice project. Instructions for building project can be found at [freeCodeCamp](https://www.freecodecamp.org/learn/apis-and-microservices/apis-and-microservices-projects/request-header-parser-microservice).

## Overview

The **Request Header Parser Microservice** is a simple API that extracts and returns information about the client's request headers. This microservice is useful for identifying and understanding the client's environment, such as their IP address, preferred language, and user agent.

## Features

- **IP Address**: Retrieves the client's IP address.
- **Language**: Extracts the client's preferred language(s) from the request headers.
- **Software**: Provides information about the client's browser and operating system from the user agent string.

## Endpoint

### GET `/api/whoami`

#### Response

The endpoint returns a JSON object with the following properties:

- `ipaddress`: The IP address of the client.
- `language`: The preferred language(s) of the client.
- `software`: The user agent string of the client.

#### Example Response

```json
{
  "ipaddress": "192.168.1.1",
  "language": "en-US,en;q=0.9",
  "software": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36"
}
```

## How to Use

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/request-header-parser-microservice.git
   ```

2. **Install dependencies**:
   ```bash
   cd request-header-parser-microservice
   npm install
   ```

3. **Start the server**:
   ```bash
   npm run start
   ```

4. **Make a request**:
   - Open your browser or use a tool like `curl` or Postman to make a GET request to `http://localhost:3000/api/whoami`.

## Technologies Used

- **Node.js**: JavaScript runtime environment.
- **Express.js**: Web framework for Node.js.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## Contact

For any questions or feedback, please contact [yourname@example.com](mailto:yourname@example.com).
