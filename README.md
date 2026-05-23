# pytest-pipeline

A Python application demonstrating best practices for testing, linting, and code formatting with automated CI/CD using GitHub Actions.

## Requirements

- Python 3.12.13 or higher
- Make

## Dependencies

- `pytest==9.0.3` - Testing framework
- `pytest-cov==7.1.0` - Code coverage plugin for pytest
- `pylint==4.0.5` - Code linting tool
- `black` - Code formatter
- `ipython` - Interactive Python shell

## Installation

Install dependencies using Make:

```bash
make install
```

This will install all required packages from `requirements.txt` into a virtual environment.

## Usage

Run the application:

```bash
python hello.py
```

## Testing

Run tests with pytest:

```bash
make test
```

This will execute all tests in `test_hello.py` and generate a coverage report.

## Linting

Check code quality with pylint:

```bash
make lint
```

## Code Formatting

Format code with black:

```bash
make format
```

## CI/CD Pipeline

This repository includes a GitHub Actions workflow that automatically:

1. **Installs dependencies** - Sets up the Python environment and installs all required packages
2. **Lints code** - Checks code quality using pylint
3. **Runs tests** - Executes the test suite with pytest
4. **Formats code** - Verifies code formatting with black

The workflow runs on every push to the repository.

## File Structure

```
.
├── hello.py                              # Main application file
├── test_hello.py                         # Test suite
├── requirements.txt                      # Python dependencies
├── Makefile                              # Build automation
├── README.md                             # This file
└── .github/workflows/testing-ci.yml      # GitHub Actions workflow
```

## License

This project is open source and available under the MIT License.
