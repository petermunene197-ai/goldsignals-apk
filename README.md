# GoldSignals APK Documentation

## Features
- **Automatic Builds**: Integrates with GitHub Actions for continuous deployment.
- **Manual Builds**: Instructions for building the project locally.
- **Custom Indicators**: Use tailored indicators for trading signals.

## Quick Start Instructions

### GitHub Actions Automatic Build
1. **Set up GitHub Actions**: Ensure the `.github/workflows` directory contains the correct YAML configuration for builds.
2. **Push to Repository**: Any push to the main branch will trigger the GitHub Actions workflow, resulting in an automatic build.

### Manual Local Build
1. **Clone the Repository**: Run `git clone https://github.com/petermunene197-ai/goldsignals-apk.git`
2. **Install Dependencies**: Use the package manager to install required libraries:
   ```bash
   cd goldsignals-apk
   npm install
   ```
3. **Build the APK**: Execute the build command:
   ```bash
   npm run build
   ```
4. Find your built APK in the `dist` folder.

## Installation Methods
- **Android Device**: Transfer the APK file to your device and install it, ensuring that installations from unknown sources are enabled.
- **Emulator**: Use an Android emulator to run the APK file directly.

## Indicator Weights
- **Weighting System**: Each indicator's signal is weighted based on historical performance, ranging from 0 to 1 where 1 indicates the highest confidence.

## Signal Confidence Levels
- **Levels**: Signals are rated from 0 to 100%, indicating the likelihood of success based on past data and algorithm predictions.
- **Visualization**: Signal confidence is shown clearly in the application interface, allowing users to make informed decisions.

## API Reference
- **Endpoint**: `/api/signals`
- **Methods**: `GET` for fetching current signal data.
- **Response Format**:
  ```json
  {
    "signals": [
      {
        "indicator": "EMA",
        "confidence": 90,
        "weight": 0.8
      }
    ]
  }
  ```

## Disclaimer
This project provides trading signals based on algorithmic analysis but does not guarantee profits. Use at your own risk.

## Support Information
For support, issues, or feature requests, please open an issue on GitHub or contact us at support@goldsignals.com.