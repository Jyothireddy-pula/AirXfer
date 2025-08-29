
AirXfer – Gesture-Based File Transfer
🌟 About the Project

built with the idea of making file sharing between two computers easier and more interactive. Instead of clicking buttons or using cables, I wanted to try something unique: controlling file transfer with hand gestures.

This project combines computer vision (hand gesture recognition) with networking (UDP + TCP sockets) to create a working prototype of “gesture-controlled AirDrop.”

🔹 Features

Gesture Recognition: Uses MediaPipe Hand Tracking to detect hand gestures.

Wireless File Transfer: Sends files directly between PCs without external apps.

Auto Device Discovery: The sender detects the receiver’s IP automatically.

Buffer + Storage: Files are buffered first and then stored safely in the receiver’s Downloads folder.

Simple Prototype: Focused on functionality more than design (since it’s my first build).

🔹 How It Works (Simple Explanation)

Receiver side: broadcasts its availability using UDP.

Sender side: listens for this broadcast and gets the receiver’s IP address.

A TCP connection is established between sender and receiver.

Sender transfers the files → receiver buffers them → saves them in Downloads.

Hand gestures are used to trigger or control the sending process.

🛠️ Tech Stack

Programming Language: Python

Computer Vision: MediaPipe Hand Tracking

Networking: UDP (discovery) + TCP (file transfer)

OS Support: Works on Windows/Linux (tested locally)

🔹 Challenges I Faced
 I faced many challenges:

Learning how UDP and TCP sockets actually work.

Integrating gesture recognition with file transfer logic.

Handling buffering and storage so files don’t get corrupted.

Debugging networking issues when sender and receiver didn’t connect properly.

But overcoming these gave me a lot of confidence in combining AI + networking.


🚀 Future Improvements

Add more gesture commands (pause/resume transfer, cancel, multiple file selection).

Create a GUI instead of only console-based interface.

Add encryption for secure transfers.

Optimize speed for larger files.





© 2025 JYOTHI REDDY PULA . All Rights Reserved.  
This project is not licensed for free use. Contact for permissions.
