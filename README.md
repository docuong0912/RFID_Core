SETUP in VS IDE (purple icon):
  - install .net 6.0 SKD in https://dotnet.microsoft.com/en-us/download/dotnet/6.0
  - or .net 7.0SDK https://dotnet.microsoft.com/en-us/download/dotnet/7.0
  - or any preference version
  With upgrade:
  - Install the .NET Upgrade Assistant in https://marketplace.visualstudio.com/items?itemName=ms-dotnettools.upgradeassistant
  - open sln of RFID1 project
  - right click on the project > select Upgrade > Side-by-side project upgrade > New project > Change project name(if needed) > click Next > Select .net6.0 SDK or .net7.0SDK(Preferenced)(required installed SDK in above step) > Upgrade selection> Wait to completed
  ![alt text](https://github.com/docuong0912/RFID_Core/blob/main/images/upgrade.png?raw=true)
  - Go to step 2 below
  Without upgrade:
  - Clone this project to the same directory of original RFID1 project
  - Reference STUHFL_cs.dll from original .net framework project by right-click on dependency tab  click "Add project reference..."
  - go to tab Browse > Navigate to STUHFL_cs.dll of original project> select the file > click Add
  - Click OK on Reference Manager window
  - run the project
ERROR:
- Handle Error	CS0103	The name 'SerialPort' does not exist in the current context	RFIDCore:
    - click on bulb icon(hint) >Install package 'System.IO.Ports'> Find and install latest version
