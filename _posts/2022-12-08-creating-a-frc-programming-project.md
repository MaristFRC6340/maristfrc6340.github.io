## Creating a FRC Programming-Project

Creating an FRC project involves using VS Code, so make sure you have the WPILib Visual Studio Code installed!

In this blog post, you will learn out to:
* Create a project in VS Code
* Initialize a basic command based project
* Create a "Robot" with a drivetrain subsystem

---

> **Creating a Command Based Repository**
1. Open Visual Studio and Create a new Command Based Project **(Follow [this guide](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-4/creating-benchtop-test-program-cpp-java.html) but select "Command Based")**

![new project img](https://firstmncsa.files.wordpress.com/2018/09/vsc_program_palette.png)

> **Initializing a robot in your repository**
1. Setup the `Robot.jav`a class with Joystick static objects and Accessors. 
[Example](https://github.com/MaristFRC6340/2022ProtoCode/blob/master/src/main/java/frc/robot/Robot.java)

> **Creating a `DriveTrain.java` subsystem**
1. *Right click* on the source folder where you want to code and press *New File*
2. Create a `DriveTrain.java` subsystem. Examples: [2017:](https://github.com/MaristFRC6340/2022ProtoCode/tree/master/src/main/java/frc/robot) & [2020:](https://github.com/MaristFRC6340/2022NeoBaseCode/tree/master/src/main)

![create file](https://camo.githubusercontent.com/87dd1eb9a5f8f778729c9654a51efab27cbdff8f5f36871e8d962281b781ab01/68747470733a2f2f636c6475702e636f6d2f57316744656b334537442e706e67)

> **Setup `RobotContainer.java` file**
1. Create a `Field` for `TankDrive`
2. Create an `Accessor` for Field of `TankDrive` instance

> **Finish Creating the Robot Class**
1. Create instance of RobotContainer
2. Schedule the DriveTrain command

![image](https://user-images.githubusercontent.com/44009231/167966154-164c48f9-f291-4f25-bd9c-920a45392d91.png)

---

### Things to consider

To build the project, simply click on the WPILib Logo (with a "W") in the top right corner and it will *build* the code. However, to deploy the code
to the RoboRIO is an entirely different process not covered in this video.

![building code](https://user-images.githubusercontent.com/44009231/206465061-4c8d0f18-7092-4444-b104-e8ba7f2befe7.png)

**NOTE: To setup this repository with Github and Version Control, *see [this guide!](https://maristfrc6340.github.io/2021/03/08/version-control-for-robot-code.html)***

---

<h4 align="center"> Created by Alessio Toniolo </h4>
