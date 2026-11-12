# Oshi Extension: Sample Template

[![Oshi Compatible](https://img.shields.io/badge/Oshi-Extension-7c3aed.svg)](https://github.com/Ogaku/Oshi)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Starter template and documentation for building an **Oshi Provider Extension**.

## How to create your own extension
Each extension is a single Dart script executed inside Oshi via d4rt (Dart runtime interpreter).

1. Define metadata header at top of extension.dart:
   `dart
   // @id PROVGUID-MY-REGISTER
   // @name My School Register
   // @version 1.0.0
   // @author YourName
   // @baseUrl https://myregister.example.com
   `
2. Implement required lifecycle hooks:
   - Future<Map<String, dynamic>> login(Map<String, String> credentials)
   - Future<Map<String, dynamic>> refresh({String? weekStart})
   - Map<String, dynamic> getRegisterDataJson()
3. Publish in your own GitHub repository!
4. Submit your extension to [Ogaku/Oshi-Extensions](https://github.com/Ogaku/Oshi-Extensions).
