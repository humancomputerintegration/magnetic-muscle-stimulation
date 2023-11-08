# Interactive Benefits from Switching Electrical to Magnetic Muscle Stimulation

This is the repository for software instances (Python script) used for the "Interactive Benefits from Switching Electrical to Magnetic Muscle Stimulation" paper (ACM UIST2023).

For more information, please refer to our paper: https://lab.plopes.org/#MMS

# how to use
The code sets up an OSC server that sends serial messages to the magnetic stimulator in response to OSC messages from any OSC clients held in other program instances such as Unity, Python, Processing, etc.

For controlling the serial messages to the stimulator, our program uses MagPy Python Toolbox (https://github.com/nicolasmcnair/magpy), so please install this prior to run our Python script.

reference: Nicolas A McNair. 2017. MagPy: A Python toolbox for controlling Magstim transcranial magnetic stimulators. Journal of neuroscience methods 276 (2017).

For hardware connection between your laptop and the stimulator, you need to have a usb-to-DB-26M cable; please refer to this page for more details https://github.com/nicolasmcnair/magpy/wiki/The-Serial-Cable

Once you have MagPy and the hardware connection established, now you need to configure:  
(1) the serial port of your laptop connected to the stimulator (line67)  
(2) the 4-8-2-digit unlock code that comes with your Magstim stimulator (line67)  
(3) ip address and OSC port names (line9-13) on our script and your script that communicates with our script.  

## notes
Currently, our software pipeine is only compatible with a medical-grade magnetic stimulator (Magstim Super Rapid^2). We hope to release an open-source custom magnetic stimulator someday in the future; so please stay tuned!

# citing
When using or building upon this device in an academic publication, please consider citing as follows:

Yudai Tanaka, Akifumi Takahashi, and Pedro Lopes. 2023. Interactive Benefits from Switching Electrical to Magnetic Muscle Stimulation. In Proceedings of ACM Symposium on User Interface Software and Technology 2023 (UIST ’23). Association for Computing Machinery, New York, NY, USA. DOI:10.1145/3586183.3606812

# contact
For any questions about this repository, please contact yudaitanaka@uchicago.edu
