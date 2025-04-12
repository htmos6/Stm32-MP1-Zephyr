**Zephyr Project Setup Guide (Windows – PowerShell)**

Follow these simple steps toset up your Zephyr environment on Windows using PowerShell.

**Step 1: Open a Terminal**

*   Open **PowerShell** or **Command Prompt** (cmd.exe) as a **regular user** (not as Administrator).
    

**Step 2: Navigate to Your Project Folder & Create a Virtual Environment**

The **.venv** folderwill contain your **Python virtual environment**.

**Step 3: Activate the Virtual Environment**

**Important:** You needto **activate** the **virtual** **environment** **everytime** you open a new terminal and work on this project.

**Step 4: Install West (Zephyr's project manager tool)**

Once the virtual environmentis activated, install West with:

**Step 5: Initialize Zephyr in the Workspace**

Make sure you're in thecorrect folder:

Then initialize Zephyrproject named as **Zephyr-Src**and fetch Zephyr source code:

**Step 6: Organize the Folder Structure**

Organize the Folder Structure

**Step 6: West Update**

Make sure you're in thecorrect folder.Then update Zephyr source code.

**Step 7: Export ZephyrCMake Package**

Export Zephyr’s CMake package. Thisenables CMake to locate and load the required boilerplate automatically whenbuilding applications

**Step 8: Install Python Dependenciesfrom Zephyr Packages**

Use the **west packages** command to install allPython requirements defined by Zephyr modules.

**Step 9: Install the ZephyrSDK**

The Zephyr Software Development Kit (SDK)includes compilers, linkers, debuggers, and other essential tools for buildingand debugging applications across Zephyr's supported architectures.

To install the SDK on Windows usingWest:

**Step 10: Build the BlinkySample**

To view the list of supported boards,run.

Once you've identified yourboard, you can build the Blinky example application. Replace with your actual board identifier:

**west build -p always -b stm32mp157c\_dk2 samples\\basic\\blinky**