Here is the `README.md` content within a single code block:

```md
# Project Installation and Setup Guide

## Prerequisites

- Ensure that you have [Node.js](https://nodejs.org/) installed.
- Install [Yarn](https://classic.yarnpkg.com/en/docs/install/#mac-stable) package manager.
- Install [PM2](https://pm2.keymetrics.io/docs/usage/quick-start/) globally for process management.

## Installation Steps

1. **Clone the repository**:
   ```bash
   git clone <your-repository-url>
   cd <your-repository-folder>
   ```

2. **Install dependencies in the root folder**:
   Open your terminal and navigate to the root folder of your project. Then run:
   ```bash
   npm i -g yarn
   yarn
   ```

3. **Install dependencies in the server folder**:
   Navigate to the `server` directory and install the necessary dependencies:
   ```bash
   cd server
   yarn
   ```

4. **Download the required JSON file**:
   In the `server` directory, download the following JSON file and place it in the appropriate location:
   - [https://api.raydium.io/v2/sdk/liquidity/mainnet.json](https://api.raydium.io/v2/sdk/liquidity/mainnet.json)

5. **Return to the root directory**:
   After setting up the server, navigate back to the root directory:
   ```bash
   cd ..
   ```

6. **Install PM2 globally**:
   Install PM2 globally using the following command:
   ```bash
   npm i pm2 -g
   ```

7. **Start the application using PM2**:
   Finally, start the application using PM2:
   ```bash
   pm2 start ecosystem.config.js
   ```
```
