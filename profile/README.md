# Phone Number Tracker

Phone Number Tracker can be used to perform a completely free reverse phone lookup for any Indian or US phone number. Simply enter the phone number in the form below and click the search button to get the owner's full name and more details. Firm registration and API setup is required to get the owner's full name. We are 100% non-corporate and non-negotiable. We guarantee you that you will not find a more accurate phone number lookup service.

Visit the website for more details and demo: Developers can get the telecom operator and some other details by the code given below.

Check Live Demo : - [Phone Number Tracker](https://www.mobilenumbertracker.in)

---

## Project Overview

The **Mobile Number Tracker CLI** is a powerful tool designed to facilitate phone number validation, service provider lookup, and random location coordinate generation. This package offers an easy-to-use command-line interface (CLI) and programmatic access via JavaScript.

### Key Features

- **Phone Number Validation**: Ensures whether a given phone number follows the correct format.
- **Service Provider Lookup**: Retrieves telecom provider details based on the country code.
- **Location Coordinate Generator**: Generates random latitude and longitude coordinates.
- **Command-Line Interface (CLI)**: Provides quick access to package functionalities without writing code.

---

## Project Structure

The project is organized into the following directories and files:

```
tracker/
|-- bin/                            # Command Line Interface
|   |-- cli.js                      # CLI script for using the package
|-- src/
|   |-- index.js                    # Main module for the package
|   |-- validator.js                # Phone number validation functions
|   |-- provider.js                 # Service provider information
|   |-- locationGenerator.js        # Location coordinates generator
|-- CODE_OF_CONDUCT.md
|-- LEARN.md
|-- CONTRIBUTING.md
|-- package.json                    # Package configuration
|-- README.md                       # Package documentation (you are here)
|-- LICENSE                         # License file
```

---

## Installation Guide

To install the **Mobile Number Tracker CLI** package globally using npm, run:

```sh
npm install -g mobile-number-tracker
```

---

## Usage Examples

### Validate a Phone Number

To check if a phone number is valid:

```javascript
const phoneTracker = require("mobile-number-tracker");

const phoneNumber = "+19999999999";
const isValid = phoneTracker.isValidPhoneNumber(phoneNumber);
console.log(`Is Valid: ${isValid}`);
```

### Get Service Provider Information

To retrieve telecom provider details based on a country code:

```javascript
const phoneTracker = require("mobile-number-tracker");

const countryCode = "+1";
const serviceProvider = phoneTracker.getServiceProvider(countryCode);
console.log(`Country Code: ${countryCode}`);
console.log(`Service Provider: ${serviceProvider}`);
```

### Generate Random Coordinates

To create random latitude and longitude values:

```javascript
const phoneTracker = require("mobile-number-tracker");

const randomLocation = phoneTracker.generateRandomLocation(-90, 90, -180, 180);
console.log(`Latitude: ${randomLocation.latitude}`);
console.log(`Longitude: ${randomLocation.longitude}`);
```

---

## Command Line Interface (CLI) User Guide

The package provides a CLI for easy functionality access. Here are some common use cases:

### Validate a Phone Number

```sh
phone-tracker -v +19999999999
```

### Get Service Provider Information

```sh
phone-tracker -s +1
```

### Generate Random Coordinates

```sh
phone-tracker -c
```

---

## License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

---

## Conclusion

The **Mobile Number Tracker CLI** is an efficient and user-friendly package for validating phone numbers, retrieving service provider details, and generating random location coordinates. Whether you're a developer looking for programmatic solutions or a CLI user needing quick access to phone data, this package provides a seamless experience.
