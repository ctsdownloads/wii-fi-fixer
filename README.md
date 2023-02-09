# wi-fi-fixer
Linux Wi-Fi script for detecting and fixing common Intel wifi issues

## (Check back periodically for updates) 


## Detects and fixes common issues with Intel wifi on GNOME environments:

- Logic provided to be downloaded on one computer, then run onto another.
- Checks if the wifi radio is off, turns it on.
- Restarts NetworkManager if down, then fixes it by restarting NetworkManager (GNOME).
- Checks for Airplane mode. turns it off.
- Checks for Intel wifi modules, if not loaded - detects and loads them.
- Once setup, this little script will tell you if you're connected to the wrong Wi-Fi WAP.



## From a computer that has internet (Just copy, paste and enter - that's it!)

- [Open this Gist link](https://gist.githubusercontent.com/ctsdownloads/662eda6d544403aa0392f87c8a9ae7ae/raw/2b6a08c3d60e6da53357bbb387a9bfc41f398d2e/wifi-fixer-downloader) , Ctrl A, paste the entire code block into a terminal. It's okay to include the comments, still works.

- Follow the directions that appear after the command is run.



## From the computer that needs the Wi-Fi fixed (Just copy, paste and enter - that's it!)

- Insert USB flash drive with your newly created/customized wi-fi-fixer.tar.gz file.
- Copy it to the laptop's home directory that you would like to have Wi-Fi fixed on.
- Open a terminal and paste in the following:

```cd wi-fi-fixer/ && chmod +x wifi-fixer-bash-script.sh && sh wifi-fixer-bash-script.sh```




## Troubleshooting

- Can't find NetworkManager errors? This was tested on Ubuntu GNOME. Should work on any GNOME desktop (MATE?). You can edit and replace sudo systemctl restart NetworkManager with whatever works best for your desktop environment.

- It's telling me I'm on the wrong WAP! Well, are you? If you didn't edit the file and follow step 3 above, do so.





## Examples

In Airplane mode:
[![asciicast](https://asciinema.org/a/557456.svg)](https://asciinema.org/a/557456)

No driver modules loaded for Intel wireless:
[![asciicast](https://asciinema.org/a/557452.svg)](https://asciinema.org/a/557452)

WiFi Connected to the wrong WAP (router):
[![asciicast](https://asciinema.org/a/557458.svg)](https://asciinema.org/a/557458)

Updated..Added Power Save Indicator (useful if unsure):
[![asciicast](https://asciinema.org/a/557462.svg)](https://asciinema.org/a/557462)

