# Solana Wallet Checker: Search for Wallets with Balances

Looking to discover Solana wallets with existing balances? **SolanaChecker** includes a powerful feature to search for wallets by generating and checking random seed phrases. This is ideal for research, and potentially finding active wallets.

<p align="left">
    <img src="/branding/middle.webp" />
</p>

## Key Features

1.  **Solana Balance Check:** Check the balance on a specific Solana address.

<p align="left">
    <img src="/branding/accent.webp" />
</p>

2.  **Token Security:** Analyze token security.

<p align="left">
    <img src="/branding/flat.webp" />
</p>

3.  **Address Tracking (Telegram):** Get Telegram notifications.

4.  **Mnemonic Extraction:** Retrieve data.

<p align="left">
    <img src="/branding/black.webp" />
</p>

5.  **Solana Wallet Generation:** Create wallets.

<p align="left">
    <img src="/branding/screen.webp" />
</p>

6.  **Brute-Force Search for Solana Wallets (with Telegram):**  The core search feature.  Find wallets with a balance (for research purposes), and with optional Telegram notification support.

<p align="left">
    <img src="/branding/new.webp" />
</p>

## Telegram Setup

To get Telegram alerts, put your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in 'telegram-settings.txt'.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

The project is built with C++ and uses libraries.  **vcpkg** is recommended:

### Installing Dependencies with vcpkg

1.  If you don't have **vcpkg**, install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add the **vcpkg** installation path to your system's PATH.
3.  Run these commands:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  Build the project.

### Building with Visual Studio

1.  Open the solution in Visual Studio.
2.  Ensure **vcpkg** is integrated (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  Executable in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line

1.  **-s / -search**: Start the brute-force wallet search.
2.  **-t / -track (ADDRESS)**: Track an address.
3.  **-g / -gen (NUMBER)**: Generate wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Show wallet data.
5.  **-b / -balance (ADDRESS)**: Show balance.

## Important Notes

-   Research only; no illegal use.
-   Crypto is risky; protect your data.

## License

This project is under the [MIT License](/LICENSE).

Update:  16.06.2025