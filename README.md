# Project Structure

This document provides an overview of the project structure for the `pump_anchor` Rust project.

## Directory Layout

```
pump_anchor/
├── migrations/
│   └── deploy.sh
├── programs/
│   └── solana_program.rs
├── target/
│   └── keypair.json
├── tests/
│   ├── components/
│   │   ├── header_test.rs
│   │   ├── footer_test.rs
│   │   └── sidebar_test.rs
│   ├── services/
│   │   ├── api_service_test.rs
│   │   └── auth_service_test.rs
│   └── utils/
│       ├── helpers_test.rs
│       └── constants_test.rs
│   └── unit_test.rs
├── Cargo.toml
├── Cargo.lock
└── README.md
```

## Directories

- **migrations/**: Contains deployment scripts.
  - **deploy.sh**: Script for deploying the project.

- **programs/**: Contains Solana program source code.
  - **solana_program.rs**: Source code for the Solana program.

- **target/**: Contains deployment keypair.
  - **keypair.json**: Keypair for deployment.

- **tests/**: Contains test files for the project.
  - **components/**: Tests for modules and components.
  - **services/**: Tests for service modules.
  - **utils/**: Tests for utility functions.
  - **unit_test.rs**: Unit test script.

- **src/**: Contains the source code of the project.
  - **components/**: Reusable modules and components.
  - **services/**: Modules for API calls and authentication.
  - **utils/**: Utility functions and constants.
  - **main.rs**: Entry point of the application.
  - **lib.rs**: Library module for the project.

- **Cargo.toml**: Contains project metadata and dependencies.
- **Cargo.lock**: Lock file for dependencies.
- **README.md**: Project documentation (this file).

## Getting Started

To get started with the project, follow these steps:

1. Clone the repository:
   ```sh
   git clone <repository-url>
   ```

2. Build the project:
   ```sh
   cd pump_anchor
   cargo build
   ```

3. Run the application:
   ```sh
   cargo run
   ```

## Running Tests

To run the tests, use the following command:
```sh
cargo test
```

## Deploying

To deploy the project, navigate to the `migrations` folder and run the deploy script:
```sh
cd migrations
./deploy.sh
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

## Additional Information

This project is designed to provide a robust and scalable architecture for building Rust applications. The `src` directory contains all the main code, organized into components, services, and utilities to ensure modularity and reusability. The `tests` directory includes unit tests to maintain code quality.

For more detailed documentation on each module and component, please refer to the inline comments and documentation within the respective files.