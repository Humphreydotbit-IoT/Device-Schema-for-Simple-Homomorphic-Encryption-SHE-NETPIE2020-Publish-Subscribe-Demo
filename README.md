# Device-Schema-for-Simple-Homomorphic-Encryption
## Overview

This project defines a JSON schema for device operations involving simple homomorphic encryption (SHE). The schema specifies properties and operations that can be performed on encrypted data, including storing data with a time-to-live (TTL) and performing basic arithmetic transformations such as multiplication and addition.

## Schema Details

### Properties

- **c1**: 
  - **Operation**: Store with a TTL of 7 days.
  - **Transform**: Identity transformation (`$.c1`).
  - **Type**: Number

- **c2**: 
  - **Operation**: Store with a TTL of 7 days.
  - **Type**: Number

- **multiplication**:
  - **Operation**: 
    - Store with a TTL of 7 days.
    - Transform: Multiplication of `c1` and `c2` (`$.c1 * $.c2`).
  - **Type**: Number

- **additive**:
  - **Operation**: 
    - Store with a TTL of 7 days.
    - Transform: Addition of `c1` and `c2` (`$.c1 + $.c2`).
  - **Type**: Number

## Usage

This schema can be used in applications involving simple homomorphic encryption to define operations and transformations on encrypted data. The operations ensure that data is stored with a specific time-to-live and that basic arithmetic transformations can be performed on the encrypted data.

# NETPIE2020 Publish/Subscribe Demo

## Overview

This project demonstrates the use of the NETPIE2020 platform for publishing and subscribing to messages using the MQTT protocol. NETPIE2020 is an IoT platform that facilitates the connection and management of IoT devices.

## Notebook Details

### Features

- **Connect to NETPIE2020**: Establish a connection to the NETPIE2020 service using provided credentials.
- **Publish Messages**: Send messages to a specified topic.
- **Subscribe to Messages**: Listen for messages from a specified topic and process them accordingly.

## Usage

### Prerequisites

- NETPIE2020 account and credentials.
- MQTT library (e.g., `paho-mqtt`).

### Running the Notebook

1. Install required packages:
   ```bash
   pip install paho-mqtt
# Somewhat Homomorphic Encryption Toy Example

## Overview

This project provides a toy example of somewhat homomorphic encryption (SHE) using a Jupyter notebook. Homomorphic encryption allows computations to be carried out on ciphertext, generating an encrypted result which, when decrypted, matches the result of operations performed on the plaintext.

## Notebook Details

### Features

- **Encrypt Data**: Encrypt numerical data using homomorphic encryption.
- **Perform Arithmetic Operations**: Perform basic arithmetic operations (addition, multiplication) on encrypted data.
- **Decrypt Data**: Decrypt the results to verify the correctness of the operations performed on the ciphertext.

## Usage

### Prerequisites

- Python environment with Jupyter installed.
- Libraries for homomorphic encryption (e.g., PySEAL, TenSEAL).

### Running the Notebook

1. Install required packages:
   ```bash
   pip install PySEAL TenSEAL
