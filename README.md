# Rustonomy
- Download the Rust Server files: http://files.facepunch.com/2Fgarry/2F1b1011b1/2FRust_Server.zip
- Edit Run_DS.bat change the server name
- Run Run_DS.bat
- Run update.bat
- Install Oxide http://oxidemod.org/downloads/
- Overwrite the RustDedicated_Data with the oxide RustDedicated_Data
- Edit Run_DS.bat and paste in:

echo off
:start
cd rustds
RustDedicated.exe -batchmode +server.hostname "Rustonix Dev Server" +server.port 28015 +server.identity "my_server" +server.seed 1234567 -logFile "output.txt"
cd ../

goto start

- Run the Server
- You now have an oxide directory located in Server/rustds/
- Move the oxide plugins (pulled from this repository) to replace that directory
- Restart the Server
- Connect to the server by launching the Rust Client, F1, client.connect localhost:28015

# Issue Tracking
https://trello.com/b/E23uwXsa/rustonix
