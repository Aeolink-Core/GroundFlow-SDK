# GroundFlow-SDK
Graphic UI SDK for GroundFlow

![groundflow](https://github.com/Aeolink-Core/GroundFlow-SDK/assets/151231496/df9947c6-ab0e-411a-bb87-3c4aedb6f121)
![aeolink](https://github.com/Aeolink-Core/GroundFlow-SDK/assets/151231496/e39a0d1e-4ecb-4baf-a42c-68bbebee6483)

## Introduction
The GroundFlow SDK provides a robust framework for developing graphical user interfaces (GUIs) in applications running on the LinkOS platform. Tailored for both novices and professionals, this SDK offers a diverse set of tools that simplify the creation of rich, responsive, and visually striking UI components.

## Prerequisites
Before you begin, ensure that you have the following prerequisites installed:
- C/C++ Compiler (such as GCC or Clang)
- LinkOS Development Environment
- GroundFlow SDK libraries and header files

## Installation
To install the GroundFlow SDK, follow these steps:

1. Clone the SDK repository:
   ```bash
   git clone https://github.com/Aeolink-Core/GroundFlow-SDK.git

2. Navigate to the SDK directory:
   ```bash
   cd GroundFlow-SDK

## Implementing Your Application
Here's a simple example of how a GroundFlow application could be structured in C:

  ```c
  #include "groundflow/application.h"
  #include "groundflow/ui_component.h"

  int main() {
      gf_initialize();

      GFWindow* window = gf_create_window("My Application", 800, 600);
      gf_window_show(window);

      while (gf_is_running()) {
          gf_process_events();
          // Your application logic goes here
      }

      gf_cleanup();
      return 0;
  }
  ```

3. To compile your application, you might run:
     ```bash
     gcc main.c -o my_app -lgroundflow -I/path/to/GroundFlow-SDK/include
     ```
4. To install application on your computer, you might run:
   ```bash
   ./app-name
   ```
Documentation
For detailed documentation, see the docs directory within this repository. It includes comprehensive guides and API references.

Support
For support, please open an issue on this GitHub repository.

License
The GroundFlow SDK is licensed under the Apache 2.0 . See the LICENSE file for more details.

