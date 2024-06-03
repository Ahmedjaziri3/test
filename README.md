how to use and run test scripts for Chrome, Edge, and Safari, as well as mobile testing for iOS and Android using Appium Server.

```markdown
# Automated Testing Setup and Execution

This repository contains automated test scripts for web browsers (Chrome, Edge, Safari) and mobile devices (iOS, Android) using Selenium and Appium.

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Setup](#setup)
3. [Running Web Tests](#running-web-tests)
    - [Chrome](#chrome)
    - [Edge](#edge)
    - [Safari](#safari)
4. [Running Mobile Tests](#running-mobile-tests)
    - [iOS](#ios)
    - [Android](#android)
5. [Directory Structure](#directory-structure)
6. [Contributing](#contributing)
7. [License](#license)

## Prerequisites

- Node.js and npm
- Java Development Kit (JDK)
- WebDriver for Chrome, Edge, and Safari
- Appium Server
- Xcode (for iOS testing)
- Android SDK (for Android testing)

## Setup

1. **Clone the Repository**

   ```sh
   git clone https://github.com/Ahmedjaziri3/test
  
   ```

2. **Install Dependencies**

   ```sh
   npm install
   ```

3. **Download WebDrivers**

   - **ChromeDriver**: [Download ChromeDriver](https://sites.google.com/a/chromium.org/chromedriver/)
   - **EdgeDriver**: [Download EdgeDriver](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/)
   - **SafariDriver**: Safari comes with a built-in driver. Ensure 'Allow Remote Automation' is enabled in Safari's Develop menu.

4. **Install Appium**

   ```sh
   npm install -g appium
   ```

5. **Start Appium Server**

   ```sh
   appium
   ```

## Running Web Tests

### Chrome

1. **Start ChromeDriver**

   ```sh
   ./path/to/chromedriver
   ```

2. **Run Test Script**

   ```sh
   node tests/web/chromeTest.js
   ```

### Edge

1. **Start EdgeDriver**

   ```sh
   ./path/to/edgedriver
   ```

2. **Run Test Script**

   ```sh
   node tests/web/edgeTest.js
   ```

### Safari

1. **Enable Remote Automation in Safari**

   - Open Safari
   - Go to Safari -> Preferences -> Advanced
   - Check 'Show Develop menu in menu bar'
   - Go to Develop -> Allow Remote Automation

2. **Run Test Script**

   ```sh
   node tests/web/safariTest.js
   ```

## Running Mobile Tests

### iOS

1. **Ensure Xcode is installed and configured**

2. **Run Test Script**

   ```sh
   node tests/mobile/iosTest.js
   ```

### Android

1. **Ensure Android SDK is installed and configured**

2. **Run Test Script**

   ```sh
   node tests/mobile/androidTest.js
   ```

## Directory Structure

```
.
├── README.md
├── package.json
├── tests
│   ├── web
│   │   ├── chromeTest.js
│   │   ├── edgeTest.js
│   │   └── safariTest.js
│   └── mobile
│       ├── iosTest.js
│       └── androidTest.js
└── webdriver
    ├── chromedriver
    ├── edgedriver
    └── safaridriver
```

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.


## Notes

- Ensure all necessary WebDriver binaries are correctly placed in the `webdriver` directory.
- Adjust paths and versions according to your environment.
- Ensure that the Appium server is running before executing mobile tests.
