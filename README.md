# GroundFlow-SDK
Graphic UI SDK for GroundFlow

![Aeolink Logo](https://github.com/Aeolink-Core/GroundFlow-SDK/assets/151231496/769fc292-b34c-4da3-aa0a-af839e62db27)
![GroundFlow Logo](https://github.com/Aeolink-Core/GroundFlow-SDK/assets/151231496/f7e5cf2c-9b37-4aec-ab2f-0f2e2a040c47)
![EEAI Logo](https://github.com/Aeolink-Core/GroundFlow-SDK/assets/151231496/1e692117-aa49-487c-807f-eb6f01dfe48b)


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

### Implementing Your Application
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

