# Hello World!

This is my very first project in github, it features a simple C++ program that prints the string "Hello, World!". It is composed of a library named ``` iostream ```, and it returns 0. Below shows how it is composed

``` cpp
#include <iostream>

int main() {

    std::cout << "Hello, World!\n";

    return 0;
}
```
## How it works

The ``` #include ``` keyword tells the computer to include a certain library, in this case, it is ``` iostream ```. Then we have the ``` main() ``` function, declared using the ``` int ``` keyword because it returns a integer at the end. Then comes the command ``` std::cout ``` (pronounced "see-out"), which means "standard character output". Then we have the <<, which means a stream of output. After that, we have the string ``` "Hello, World!" ```, which is what is being printed out as an output. Right next to that, we have ``` \n ```, which basicaly creates a new line. Finally, we have the ``` return 0; ``` command, which terminates a function and tells the program that the code finished without any errors.  

## Install G++ if needed (🍎MacOS)
If you want to run this program in your local terminal, first check if g++ is installed, if not, you can install it by running this on mac:

``` sh
brew install gcc 

ls /opt/homebrew/bin | grep g++
```
Once finished, verify installation:
``` sh
g++ --version
```
Exception: If you dont have homebrew and you are using mac, you will need to install homebrew first by running this in your terminal:

``` sh
/bin/bash -c "$(curl -fsSL https://githubusercontent.com)"
```
⚠️ Critical Step: Once the installation finishes, paste this code bellow
``` sh
echo >> ~/.zprofile
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```
## Install G++ if needed (🪟Windows)
If you use windows, you will need to follow these steps instead: 

1. Go to <a href="https://msys2.org">msys2.org</a>
2. Download the installer (named `"msys2-x86_64-20260611.exe"`)
3. Run the installer and follow the prompts
4. Keep the default installation folder (usually `C:\msys2`)
5. Install the GCC toolchain by running the code in your command prompt:

``` sh
pacman -S mingw-w64-ucrt-x86_64-gcc
```
6. Press y and hit Enter to confirm the installation
  
  Once the installation finished, you will need to add GCC to your Windows Path Environment Variable, so follow these steps:  
    
1. Open the Windows Start Menu, type "env", and select "Edit the system environment variables".

2. Click the Environment Variables... button at the bottom right.

3. Click New on the right side

4. Paste the following path: `C:\msys2\ucrt64\bin`

5. Click OK on all open windows to save the changes.

  Once you finished all of the installation, verify installation by running:

  ``` sh
  g++ --version
  ```
  ### Using G++ 

G++ is a compiler that compiles our C++ code to machine code (binary code). On either Windows or Mac, we can compile our code by running:

``` sh
g++ ./hello.cpp
```
Once g++ finishes compiling your code, you can run it by running this on mac: 

``` sh
./a.out
```
But if you use windows, you must run:

``` sh
.\a.exe
```

But, you can also add a custom output name by running the following on any OS:

``` sh
g++ ./hello.cpp -o hello
```

So now, you can run this on mac to run your program:

``` sh
./hello
```

But you must run this on windows:

``` sh
.\hello
```

Congrats! You have finished you tutorial to running your first hello world program 🎉

If you want to know more about C++, you can go to the <a href="https://cppreference.com">C++ Reference</a>.
