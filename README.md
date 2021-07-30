# cv-tool-utils
Repo for common productivity utilities for CV tools 

## 1. **`vscode-opencv-dev-config`**
`base-config-opencv` : Provides basic debug and launch configuration to get started with OpenCV C++ development on VS Code

Pre-requisites: 
1. OpenCV is installed.
2. GCC/GDB are installed
3. VSCode Extension: `C/C++` is installed and enabled.


Steps:

*Shortcut* : Make a `.vscode` folder in the project dir and copy `tasks.json`, `launch.json` and `c_cpp_properties.json` to it.

Or

1. In your project folder, use terminal and start a VS Code project with
    ```shell
    ~/path/to/your/project$ code .
    ```

2. Use `Ctrl+Shft+P` and search for `C/C++ Configurations`. This will open the extension settings tab and create a `c_cpp_properties.json` in `.vscode` folder. Either manually edit the `Include Path` and `C++ standard` or edit and paste config from [`c_cpp_properties.json`](vscode-opencv-dev-config/base-config-opencv/c_cpp_properties.json).

3. Go to `Terminal > Configure Default Build Task > C/C++: g++ build active file` and copy the contents from [`tasks.json`](vscode-opencv-dev-config/base-config-opencv/tasks.json).

4. Go to `Run > Add Configuration` and copy the contents from [`launch.json`](vscode-opencv-dev-config/base-config-opencv/launch.json)
