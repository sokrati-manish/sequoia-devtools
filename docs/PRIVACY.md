# Privacy Policy for Sequoia DevTools

**Last updated:** March 6, 2026

## Overview

Sequoia DevTools is a Chrome extension designed for developers to inspect, toggle, and manage feature flags in Sequoia applications at runtime. This privacy policy explains how the extension handles data.

## Data Collection

Sequoia DevTools does **not** collect, store, transmit, or share any personal data or browsing information.

## What the Extension Accesses

The extension injects content scripts on web pages solely to:

- Read feature flag state from the page's React Fiber tree
- Toggle boolean feature flags at the developer's explicit request
- Add custom feature flags at the developer's explicit request

All data accessed (feature flag names and values) exists only within the inspected page's runtime and is displayed locally in the DevTools panel or popup. **No data leaves your browser.**

## Host Permission (`<all_urls>`)

The extension requires content scripts to run on all URLs because developers may work across different domains (localhost, staging, production). The content scripts only interact with the page's React Fiber tree to read and modify feature flag state. They do not read, collect, or transmit any other page content.

## Data Storage

The extension does not persist any data. Feature flag state is read from the page in real time and is discarded when the DevTools panel, popup, or tab is closed.

## Third-Party Services

The extension does not communicate with any external servers, APIs, or third-party services.

## Changes to This Policy

We may update this privacy policy from time to time. Any changes will be reflected by updating the "Last updated" date above.

## Contact

If you have questions about this privacy policy, please open an issue on the project's GitHub repository.