# grrs — Rust CLI Search Tool
 
> A lightweight command-line tool written in Rust for fast and convenient pattern searching inside files.
 
---
 
## Table of Contents
 
- [Installation](#-installation)
- [Usage](#️-usage)
- [Tests](#-running-tests)
- [License](#-license)
---
 
## Installation
 
### Prerequisites
 
Before using this project, make sure **Rust** and **Cargo** are installed on your system.
 
#### 1. Install Rust and Cargo
 
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
 
Once installation is complete, restart your terminal or run:
 
```bash
source $HOME/.cargo/env
```
 
#### 2. Clone the Repository
 
```bash
git clone https://github.com/CodeStriker7/grrs.git
cd grrs
```
 
#### 3. Install Globally
 
To use `grrs` from anywhere on your system:
 
```bash
cargo install --path .
```
 
This compiles the binary and places it in `~/.cargo/bin`.
 
---
 
## Usage
 
Once installed, you can use it from any directory in the following format:
 
```bash
grrs <PATTERN> <FILE_PATH>
```
 
### Example
 
```bash
grrs "fn main" src/main.rs

echo -e "hello world\nrust is awesome\nhello rust" > test.txt
grrs "hello" test.txt
```
 
---
 
## Running Tests
 
To verify that everything is working correctly:
 
```bash
cargo test
```
 
---


