# Dbisu Raspberry Pi Pico-W USB Rubber Ducky
Dbisu's amazing tool to turn a $10 microcontroller into a world class hacking device! This is by no means my tool, 100% of credit goes to Dbisu and his extraordinary talent. ***FOR THIS TO WORK, YOU MUST BE USING A RASPBERRY PI PICO W***

### Links
Original Respository - <https://github.com/dbisu/pico-ducky>

More Payloads - <https://github.com/hak5/usbrubberducky-payloads>

How to Use Duckyscript **(Note that as of now, the Pico Ducky is only compatible with Duckyscript 1.0)** - <https://docs.hak5.org/hak5-usb-rubber-ducky/>

### Steps:
1. Download the ZIP file for this repository, and save it in a place you'll remember, or use the shell command `git clone https://github.com/responsivereality/Dbisu-Pico-W-Ducky.git`

2. While holding the **BOOTSEL** button on the Pico, plug it into your computer. It will show up as **RPI-RPI2** on your system, regardless of operating system, as is it now in bootloader mode. 

3. Decompress the ZIP, or open the folder you just cloned, and locate a file called `adafruit-circuitpython-raspberry_pi_pico_w-en_US-8.0.4.uf2`. Drag it into the root of the Pico. It will then disconnect from your computer, and reconnect automatically as **CIRCUITPY**, as it now has the latest compatible CircuitPython firmware installed

4. From here, it is the easy part. Drag `boot.py`, `code.py`, `duckyinpython.py`, the entire `lib` folder, `secrets.py`, `webapp.py`, and `wsgiserver.py` from the cloneor compressed folder from earlier into the root of the Pico's file system. It will warn you about overwriting a couple files, but ignore that and press replace

5. Now it is as simple as unplugging and replugging the Pico back into your computer. This will start the Python webserver, and you will see a new WiFi network in your toolbar called `Network`. Make sure that the Pico is plugged into a computer that you want to be affected by the script we will code together!

6. Connect to `Network` using the password `password`, and open <http://192.168.4.1:80> on your web browser. You will be met with a simple interface, from which you can view, edit and execute command files called "payloads". 

7. On the web interface, click "New", name the script payload.dd, and copy the content of `payload.txt` and paste it into the text field under the script title you just entered. Click submit, then press the button to navigate back to home. The moment you hit "Run", the script should execute on the computer the Pico is attached to, and begin playing the infamous rickroll! 

8. Have fun creating your own payloads for whatever the task requires, whether that being increasing workflow automation productivity or pranking your friends! ***Please remember that this is a hacking tool, therefore it can be used for malicious intent. Please remember never to use this tool in a harmful manner, as it may violate a law.*** Please feel free to contact me if you need any assistance whatsoever with this project!
