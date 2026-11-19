<a href="https://www.frostauth.cc/">
  <img src="https://i.imgur.com/TMQEj68.png" alt="FrostAuth. Issue keys. Control access." width="100%" />
</a>

<p align="center">
  <a href="https://www.frostauth.cc/"><img alt="FrostAuth website V.1.0.1" src="https://img.shields.io/badge/Website-V.1.0.1-6366F1?style=for-the-badge" /></a>
  <a href="https://docs.frostauth.cc/"><img alt="FrostAuth API docs" src="https://img.shields.io/badge/Docs-API_Reference-3D4695?style=for-the-badge" /></a>
  <a href="https://www.frostauth.cc/discord"><img alt="FrostAuth Discord support" src="https://img.shields.io/badge/Discord-Support-5865F2?style=for-the-badge&amp;logo=discord&amp;logoColor=white" /></a>
</p>

## Build your first integration

Create a product and a test license in the dashboard. Open the example for your language, enter the owner ID, product ID, and app version, then run it to check activation and session validation.

[Open the dashboard](https://www.frostauth.cc/dashboard) · [Read the docs](https://docs.frostauth.cc/) · [Get help on Discord](https://www.frostauth.cc/discord)

### SDKs

| SDK | Build or run | Repository |
| --- | --- | --- |
| C# | Build `FrostAuth.sln` with .NET 8. Includes console and WinForms examples. | [FrostAuth-CS-Example](https://github.com/Frost-Auth/FrostAuth-CS-Example) |
| C++ | Build the console example with CMake and libsodium. | [FrostAuth-CPP-Example](https://github.com/Frost-Auth/FrostAuth-CPP-Example) |
| Go | Run `go run ./example` from the repo root. | [FrostAuth-Go-Example](https://github.com/Frost-Auth/FrostAuth-Go-Example) |
| Java | Run `mvn clean package` with JDK 17 or newer. | [FrostAuth-Java-Example](https://github.com/Frost-Auth/FrostAuth-Java-Example) |
| JavaScript | Import `frostauth.js` in Node.js 18 or newer. | [FrostAuth-JS-Example](https://github.com/Frost-Auth/FrostAuth-JS-Example) |
| Python | Install the dependencies in `requirements.txt` and run `example.py`. | [FrostAuth-Python-Example](https://github.com/Frost-Auth/FrostAuth-Python-Example) |
| Rust | Run `cargo build --locked --release`. GitHub access is required. | [FrostAuth-Rust-Example](https://github.com/Frost-Auth/FrostAuth-Rust-Example) |

## After your app ships

Issue one key for a customer or generate a batch for a release. Set expiration dates and device limits per license. If a customer replaces their machine, reset the device binding from the dashboard. You can also revoke access and review activation history there.

Use license-only activation or let customers sign in with app accounts. Change shared app settings through variables and use product version policies to set a minimum supported build or direct users to an update.

The SDKs verify API response signatures against a pinned Ed25519 public key. When the API issues an offline assertion, the SDK can verify it locally through its signed expiry. [FrostAuth documentation](https://docs.frostauth.cc/)

## Report an SDK issue

Open an issue in the SDK repo with your runtime version, the error code, and the steps that reproduce it. Keep license keys and session tokens out of reports. For integration questions, use [FrostAuth Discord](https://www.frostauth.cc/discord).
