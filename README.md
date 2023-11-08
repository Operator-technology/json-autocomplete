# JSON Autocomplete

JSON Autocomplete is designed to complete incomplete JSON strings. It's especially effective for handling partial outputs from Large Language Models (LLMs) like OpenAI's GPT.

## Installation

Install using npm:

```bash
npm install json-autocomplete
```

Or using Yarn:

```bash
yarn add json-autocomplete
```

## Usage

Import `jsonAutocomplete` and pass incomplete JSON strings to get them completed:

```javascript
const jsonAutocomplete = require("json-autocomplete");

// Completing LLM Output
const incompleteLLMOutput = '{ "items": [ { "name": "Appl';
console.log(jsonAutocomplete(incompleteLLMOutput)); // Outputs: { "items": [ { "name": "Appl" } ] }

// Handling Incomplete Keys
const incompleteKeyJson = '{"user": { "id": 123, "nam';
console.log(jsonAutocomplete(incompleteKeyJson)); // Outputs: {"user": { "id": 123, "nam": null } }
```

## Features

- Optimized for completing JSON from LLMs like OpenAI's GPT.
- Handles a wide range of incomplete JSON formats.
- Lightweight and dependency-free.

## Contributing

Your contributions are welcome! For bug fixes, improvements, or feature additions, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
