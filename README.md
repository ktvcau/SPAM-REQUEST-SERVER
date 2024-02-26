# XIE Tool

![XIE Tool Logo](insert_image_url_here)

## Description

XIE Tool is a spam request server tool created by XIE. It allows users to simulate device access to a server using proxies and check the server's response status. This tool is helpful for testing server performance and stability under heavy loads.

## Installation

1. **Clone Repository:**
```bash
   git clone https://github.com/ktvcau/SPAM-REQUEST-SERVER.git
```

2. **Navigate to Project Directory:**
```
   cd SPAM-REQUEST-SERVER
```

3. **Install Dependencies:**
```
   npm install
```

## Usage

1. **Configuration:**

- Modify the `config.json` file to customize the tool's behavior.
  ```json
  {
    "linkToCheck": "http://example.com/page",
    "numberOfDevices": 1000,
    "consoleOutputEnabled": true
  }
  ```

- Ensure `ipOnly.txt` contains a list of proxy IP addresses without ports.

2. **Start Tool:**
```
   npm start
```

3. **Follow Prompts:**

- If `config.json` is missing or incomplete, the tool will prompt for a new URL.
- If the URL is already specified, the tool will ask whether to use it or input a new one.

4. **Monitor Output:**

- The tool will continuously send requests to the specified URL using different proxy IP addresses.
- Successful responses (status code 200) or errors will be logged to the console.

## Dependencies

- [axios](https://www.npmjs.com/package/axios): Promise-based HTTP client for Node.js
- [fs](https://nodejs.org/api/fs.html): File system module for Node.js
- [readline](https://nodejs.org/api/readline.html): Interface for reading lines of input from a readable stream

## Contributing

Contributions are welcome! Feel free to submit bug reports, feature requests, or pull requests on the [GitHub repository](https://github.com/ktvcau/SPAM-REQUEST-SERVER).

