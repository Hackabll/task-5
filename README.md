# task-5
​1. Windows Firewall (GUI Method)
​This is the easiest way to manage the firewall on a standard Windows machine.
​Steps 1 & 2: Open Tool and List Rules
​Press the Windows key and type Windows Firewall with Advanced Security, then click to open it.
​In the left pane, click Inbound Rules to see the list of current rules (your "list").
​Step 3: Add a Rule to Block Port 23 (Telnet) 
​In the right pane, click New Rule...
​Rule Type: Select Port, then click Next.
​Protocol and Ports: Select TCP and Specific local ports. Type 23 (the port for Telnet). Click Next.
​Action: Select Block the connection. Click Next.
​Profile: Check all three boxes (Domain, Private, Public). Click Next.
​Name: Give it a memorable name like Test Block Telnet 23. Click Finish.
​Step 4: Test the Block Rule 
​Open Command Prompt (CMD).
​Type the test command: telnet 127.0.0.1 23 (If Telnet Client isn't installed, you'll need to install it first via "Turn Windows features on or off").
​Expected Result: The connection attempt should fail or time out, confirming the rule is blocking traffic.
​Step 6: Remove the Test Block Rule 
​Go back to Windows Firewall with Advanced Security > Inbound Rules.
​Find the rule named Test Block Telnet 23.
​Right-click on it and select Delete. This restores the original state.
