# Yobot-pull-from-Temper1-push-to-Phant

## Statement
From a Raspberry Pi, pull temperature data from a USB Temper1 termperature sensor every {{number}} seconds and push it to a Phant stream where the URL is {{phant-url}} , the field name is {{phant-field-name}} the Public Key is {{phant-public-key}} , and the Private Key is {{phant-private-key}}. 

## Install instructions

1. Gather the hardware together for this script: Temper1 temperature sensor; Raspberry Pi computer; SD Card.
2. Burn the [Pirateship disk image](http://pirate.sh) to your SD Card.
3. Create a Phant stream to store data in. You can use http://data.sparkfun.com for a free 50mb of data for each stream you create. For a field in your Phant stream fill out `temperature` as we have just one field for this script. Make sure to save the public key, private key, and field name that Phant gives you.
4. With the Phant details in hand and a USB Memory stick, generate this script onto the USB Memory stick using Yeobot and fill out the prompts with your Wifi info and the details that you received from Phant.
```
cd /Volumes/my-usb-drive
yeobot --repository https://github.com/rjsteinert/Yeobot-pull-from-Temper1-push-to-Phant.git
```
5. Plug everything together and connect your Raspberry Pi to a power supply. 
6. Wait 15 minutes, check your Phant stream to verify data is being added to the stream.
