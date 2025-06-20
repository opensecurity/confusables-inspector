# Confusables Inspector

> **Live Tool: [https://opensecurity.github.io/confusables-inspector/](https://opensecurity.github.io/confusables-inspector/)**

A professional, offline-first security tool to inspect strings for visually confusable Unicode characters (homoglyphs) and prevent deception-based attacks.


## Overview

Confusables Inspector is a client-side security tool designed to detect and analyze visually deceptive characters in strings. It helps identify potential **IDN homograph attacks**, which are commonly used in sophisticated phishing campaigns.

The tool works by inspecting a string for Unicode characters that look identical or similar to standard ASCII characters (e.g., Cyrillic 'а' vs. Latin 'a'). It then reveals the string's true underlying **Punycode** representation, highlights the specific deceptive characters, and provides a "safe" normalized version.

## Features

-   ✅ **Homoglyph Detection:** Identifies characters that are visually confusable with their common Latin counterparts from an extensive mapping.
-   ✅ **IDN/Punycode Analysis:** Automatically converts any input containing non-ASCII characters to its Punycode `xn--...` representation to reveal its true DNS identity.
-   ✅ **100% Offline & Client-Side:** No data is ever sent to a server. All analysis happens directly in the browser, ensuring maximum privacy and security.
-   ✅ **Visual Highlighting:** Deceptive characters are highlighted directly in the input for immediate identification, with tooltips explaining the threat.
-   ✅ **Safe Normalization:** Provides a canonical, "safe" version of the string with confusable characters replaced.
-   ✅ **Zero-Dependency:** Deployed as a single, self-contained HTML file. No installation, build steps, or external dependencies are required.

## How to Use

### Online Version

The tool is publicly accessible and ready to use:

[**https://opensecurity.github.io/confusables-inspector/**](https://opensecurity.github.io/confusables-inspector/)

### Local / Offline Version

As the tool is a single HTML file, you can easily run it locally.

1.  Download the `index.html` file from this repository.
2.  Open the file in any modern web browser (e.g., Chrome, Firefox, Safari, Edge).

## Technology

This tool is intentionally built with a minimal technology stack for maximum portability, security, and longevity.

-   **Vanilla HTML5**
-   **Vanilla CSS3**
-   **Vanilla JavaScript (ES6+)**
-   Embedded Punycode.js library for IDN conversions.
