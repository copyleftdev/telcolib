# telcolib

## Overview

`telcolib` is a Python library designed for validating phone numbers across multiple countries. Utilizing regular expressions, it ensures phone numbers adhere to specific national formats.

## Features

- Validates phone numbers from a wide range of countries.
- Easily extendable to include additional countries and formats.
- Simple, straightforward API.

## Installation

To install `telcolib`, run the following command:

```bash
pip install telcolib
```

Alternatively, you can clone the repository and install it manually:

```bash
git clone https://github.com/copyleftdev/telcolib.git
cd telcolib
pip install .
```

## Usage

Here's a quick example of how to use `telcolib`:

```python
from telcolib import PhoneNumberValidator

# Create an instance of the validator
validator = PhoneNumberValidator()

# Validate a phone number
valid = validator.validate('+14445556666', 'USA')
print("Phone number is valid:", valid)
```

## Adding Custom Patterns

To add or update a country's phone number pattern:

```python
validator.add_country_pattern('CountryName', r'^\+CountryCode\d{NumberOfDigits}$')
```

## Development

### Prerequisites

- Python 3.6 or higher.

### Setting Up a Development Environment

1. Clone the repository:

    ```bash
    git clone https://github.com/copyleftdev/telcolib.git
    ```

2. Navigate to the project directory:

    ```bash
    cd telcolib
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Running Tests

To run the tests, execute:

```bash
pytest tests/
```

## Contributing

Contributions to `telcolib` are welcome! Feel free to fork the repository and submit pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback related to `telcolib`, please open an issue in the GitHub repository.

