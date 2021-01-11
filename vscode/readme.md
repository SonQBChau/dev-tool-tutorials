

## Install [VSCode](https://code.visualstudio.com/)
1. Install [Visual Studio Code](https://code.visualstudio.com/download)

![vscode for windows](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/vscode_win.jpg)

This is optional, but it is recommend to check all the boxes

![vscode boxes](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/vscode_boxes.jpg)

2. Install the [C/C++ extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools) by Microsoft. You can install the C/C++ extension by searching for 'c++' in the Extensions view (Ctrl+Shift+X).

![vscode extensions](https://raw.githubusercontent.com/misc-sonchau/dev-tool-tutorials/main/images/vscode_extensions.jpg)


## Install a compiler
Choose one of the method below:
MinGW for Windows (Recommended)
WSL for Windows
Clang for Mac (Recommended)

## Hello World
To make sure the compiler is installed and configured correctly, we'll create the simplest Hello World C++ program
Create a folder called "HelloWorld" and open VS Code in that folder
Now create a new file called `helloworld.cpp` with the **New File** button in the File Explorer or **File > New File** command.
Now paste in this source code:

```
#include <iostream>
using namespace std;

int main()
{
    cout << "Hello World" << endl;
}
```
Now press `Ctrl+S` to save the file