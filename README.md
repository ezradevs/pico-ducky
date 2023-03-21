# Dbisu Raspberry Pi Pico-W USB Rubber Ducky
Dbisu's amazing tool to turn a $10 device into a world class hacking machine! This is by no means my tool, 100% of credit goes to Dbisu and his extraordinary talent. ***FOR THIS TO WORK, YOU MUST BE USING A RASPBERRY PI PICO W***

Original Respository - <https://github.com/dbisu/pico-ducky>

### Steps:
1. Download the ZIP file for this repository, and save it in a place you'll remember, or use the shell command `git clone https://github.com/responsivereality/Dbisu-Pico-W-Ducky.git`

2. While holding the **BOOTSEL** button on the Pico, plug it into your computer. It will show up as **RPI-RPI2** on your system, regardless of operating system, as is it now in bootloader mode. 

3. Decompress the ZIP, or open the folder you just cloned, and locate a file called `adafruit-circuitpython-raspberry_pi_pico_w-en_US-8.0.4.uf2`. Drag it into the root of the Pico. It will then disconnect from your computer, and reconnect automatically as **CIRCUITPY**, as it now has the latest compatible CircuitPython firmware installed

4. From here, it is the easy part. Drag `boot.py`, `code.py`, `duckyinpython.py`, the entire `lib` folder, `secrets.py`, `webapp.py`, and `wsgiserver.py` from the cloneor compressed folder from earlier into the root of the Pico's file system. It will warn you about overwriting a couple files, but ignore that and press replace

5. Now it is as simple as unplugging and replugging the Pico back into your computer. This will start the Python webserver, and you will see a new WiFi network in your toolbar called `Network`. Make sure that the Pico is plugged into a computer that you want to be affected by the script we will code together!

6. Connect to `Network` using the password `password`, and open <http://192.168.4.1:80> on your web browser. You will be met with a simple interface, from which you can view, edit and execute command files called "payloads". 
