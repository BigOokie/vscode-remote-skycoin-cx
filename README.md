# Visual Studio Code (VSCode) Remote Development Container for Skycoin CX
This project is based in part on work from Microsoft can be found on [GitHub](https://github.com/microsoft/vscode-remote-try-go). Refer to the [License](#License) section below for acknowledgement of Microsoft licences for their original works.

# Development Containers: CX

This project lets you use the **[VS Code Remote - Containers](https://aka.ms/vscode-remote/containers)** extension in a few easy steps with the Skycoin CX programming language.

> **Note:** At this time VS Code Remote - Containers is only available as part of the Insiders build. You will need to install the Insders version of VS Code to use Remote Containers.

> **Note:** If you're following the quick start, you can jump to the [Things to try](#things-to-try) section. 

## Setting up the development container

Follow these steps to open this sample in a container:

1. If this is your first time using a development container, please follow the [getting started steps](https://aka.ms/vscode-remote/containers/getting-started).  
    > I stongly suggest you get the Microsoft [vscode-remote-try-go](https://github.com/microsoft/vscode-remote-try-go) example working first. If you cannot get that working you will not be able to get the CX environment working either.

2. If you're not yet in a development container:
   - Clone this repository.
   - Press <kbd>F1</kbd> and select the **Remote-Containers: Open Folder in Container...** command.
   - Select the cloned copy of this folder, wait for the container to start, and try things out!

## Things to try

Once you have this sample opened in a container, you'll be able to work with it like you would locally.

Some things to try:

1. **Edit:**
   - Open `helloworld.cx`
   - Try adding some code and check out the language features.
2. **Terminal:** Press <kbd>ctrl</kbd>+<kbd>shift</kbd>+<kbd>\`</kbd> and type `uname` and other Linux commands from the terminal window.
   - Run the command `cx -v` to determine the version of CX running inside the remote container.
3. **Build, Run, and Debug:**
   - Open `helloworld.cx`
   - Add a breakpoint (e.g. on line 22).
   - Press <kbd>F5</kbd> to launch the app in the container.
   - Once the breakpoint is hit, try hovering over variables, examining locals, and more.
   - Continue, then open a local browser and go to `http://localhost:9000` and note you can connect to the server in the container.
4. **Forward another port:**
   - Stop debugging and remove the breakpoint.
   - Open `server.go`
   - Change the server port to 5000. (`portNumber := "5000"`)
   - Press <kbd>F5</kbd> to launch the app in the container.
   - Press <kbd>F1</kbd> and run the **Remote-Containers: Forward Port from Container...** command.
   - Select port 5000.
   - Click "Open Browser" in the notification that appears to access the web app on this new port.

## License
Copyright © BigOokie. All rights reserved.<br />

This is based on works from Microsoft Corporation which are subject to Copyright and licenced under the MIT License. 

See [LICENSE](LICENSE) and [MS-LICENCE](MS-LICENCE) in the project root for license information.
