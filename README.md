# HelloWasm - WebAssembly with Java
## Goal
The goal of this project is to generate a `.wasm` and `.js` file for WebAssembly using Java.

## Resources
This project includes the `HelloWorld.java` and `HelloWorld.html` from the [JWebAssembly example](https://github.com/i-net-software/JWebAssembly/tree/master/docs/samples/HelloWorld "JWebAssembly example"). 


The `POM.xml`contains the [JWebAssembly Maven plugin](JWebAssembly-maven) and the [JWebAssembly](https://github.com/i-net-software/JWebAssembly) compiler. 

## Prerequisites
This project has been tested with JDK 8. Make sure you have JDK 8 installed before running the project.

If you run the small application locally on the computer and not on a http server, 
you need to disable security settings of your browser:
* Firefox: Go to the URL about:config and set `security.fileuri.strict_origin_policy` to false.
* Chromium: Add `--allow-file-access-from-files` to the startup options.

## Usage
To generate the WebAssembly files, follow these steps:

1. Clone the repository
2. Build the project: `mvn clean package` (install, verify..)
3. Run `mvn jwebassembly:compile`
4. The generated `.wasm` and `.js` files will be located in the target directory.

To see the result in the browser, open the `HelloWorld.html` in the root-directory. 


