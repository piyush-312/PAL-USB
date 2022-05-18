# PAL USB
The only single sensor 360° 3D Vision System. [PAL USB](https://dreamvu.com/pal-usb/) is the only single sensor omnidirectional vision system to provide 360° stereoscopic sensing with depth perception. 

Please follow the instructions given below on any of the Nvidia Jetson embedded boards with Jetpack 4.6 to install the software.

## Steps

    curl -s --compressed "https://debashish05.github.io/debashishPPA/KEY.gpg" | sudo apt-key add -
    sudo curl -s --compressed -o /etc/apt/sources.list.d/my_list_file.list "https://debashish05.github.io/debashishPPA/my_list_file.list"
    sudo apt update
    sudo apt install palusb


Provide argument "Y" or "y" for the dependency to install. 

Then a message will be displayed on the terminal,

"Please select either (Y/N). On selecting 'Y', installation will build the whole software based on the particular Nvidia Jetson architecture and will enable higher performance. This may take a few hours to complete the installation. On selecting 'N', it will quickly build the software by using some of the pre-configured libraries provided. (Y/N)"

Based on the need follow enter the character. In case of rebuilding following are the recommended values for different Nvidia Jetson architectures.
    For Jetson Xavier NX arg2: 3500
    For Jetson Xavier AGX arg2: 8000
    For Jetson Nano arg2: 1000
            
Once complete please reboot the system.

## Documentation 
For rest of the evaluation of the PAL-USB SDK, please read the [Evaluation Manual](https://docs.google.com/document/d/e/2PACX-1vT3rc_7S621PJHJ6QuV-rR2CyXbMvPBZztaDoiPnkT_g18Gz327OOA91pf11JMkqIeK0smel81rNbNg/pub)

## Support 
If you need help or more informations check our [Help Center](https://support.dreamvu.com/portal/en/home) or join our [Community](https://support.dreamvu.com/portal/en/community/dreamvu-inc). 

## Contributing
Feel free to open an issue if you find a bug, or a pull request for bug fixes, features or other improvements.
