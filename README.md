# translate-type

Node.js module for translating text relying on the [Microsoft Cognitive Services Translator](https://docs.microsoft.com/en-us/azure/cognitive-services/Translator/translator-info-overview).

## About

This module builds upon the [Microsoft Azure Cognitive Services Translator API](https://docs.microsoft.com/en-us/azure/cognitive-services/Translator/quickstart-translate?pivots=programming-language-javascript). This API, of course, allows developers to interact with Microsoft Azure's Cognitive Services' Translator service to dynamically identify languages and perform translations.

This module allows Node.js developers to easily perform a core set of tasks using the Translator API:

- Language detection based on text
- Language translation of text to a specified language
- Retrieval of the language and language codes supported by the Translator API

## Usage

This module currently offers three main, simple functions:

1. `getLanguages()` - This returns a string representing a JSON object containing the languages supported by the Microsoft Translator API.

### Prerequisites

Usage of this module requires the user to have an account with [Microsoft Azure](https://azure.microsoft.com/en-us/free/). The user must create a *Translator Resource* in Azure, and the user must obtain the Subscription Key for the resource.

### Installation

1. Clone this repository.
2. Move/Add the newly created, local *translate-type* directory and its contents into the *Modules* directory of your **node.js** project:

```
    root
    |
    |-- bin/
    |-- modules/        # Move to this folder (as shown)
    |   |
    |   |-- translate-type/
    |       |
    |       |-- translate.js
    |       |-- package.json
    |       |-- package-lock.json
    |       |-- README.md
    |       |-- LICENSE
    |
    |-- node_modules/   # Or move here
    |-- public/
    |-- routes/
    |-- views/
    |-- app.js
    |-- package.json
    |-- package-lock.json
    |-- README.md
```

3. Update the package variables:

    - Update the `subscriptionKey` variable on line 13 of *translate.js* with your subscription key from your Microsoft Azure Translator resource.
    - Update the `serviceRegion` variable on line 14 of *translate.js* with your service region from your Microsoft Azure Translator resource.

4. From within the *translate-type* directory, run `npm install`.
5. From your Node.js project root directory, install the *translate-type* module by running `npm install ./<route-to-module>/translate-type`.
6. You should be able to reference the module in your own classes/modules:
    `const translator = require('translator');

## Resources

- [What is the Translator](https://docs.microsoft.com/en-us/azure/cognitive-services/Translator/translator-info-overview)
- [Quickstart: Use the Translator to translate text](https://docs.microsoft.com/en-us/azure/cognitive-services/Translator/quickstart-translate?pivots=programming-language-javascript)
- [Translator Documentation](https://docs.microsoft.com/en-us/azure/cognitive-services/Translator/)