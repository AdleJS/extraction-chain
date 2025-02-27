# Extraction Chain

This project demonstrates how to use the `@langchain/core` and `@langchain/ollama` libraries to extract structured information from text using a language model.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/extraction-chain.git
    cd extraction-chain
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

## Usage

To run the extraction script, use the following command:
```sh
node main.js
```

## Example

The script extracts information about people from a given text. For example, given the text:
```
My name is Jeff, my hair is black and I am 2 meters tall. Anna has the same color hair as me.
```

The output will be:
```json
{
    "people": [
        {
            "name": "Jeff",
            "hair_color": "black",
            "height_in_meters": 2
        },
        {
            "name": "Anna",
            "hair_color": "black",
            "height_in_meters": null
        }
    ]
}
```

## License

This project is licensed under the MIT License.