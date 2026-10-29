# Kwon Input Overlay

Shows your mouse on a pad and your keyboard next to it. It's a browser
source, so it works in OBS, Meld Studio, or anything else that takes one.
The examples below use OBS.

You give it your pad size in mm and your mouse DPI, so the dot ends up
where your hand actually is.

## Download

[Latest version](../../releases/latest)

One exe, no installer. Windows will say it doesn't recognise the app:
**More info**, then **Run anyway**. It isn't signed.

## Single PC setup

1. Run the exe.
2. Leave **Setup** on **Single PC**.
3. Press **Start**.
4. Press **Copy** next to **browser source**.
5. Paste it into a Browser source in OBS.
6. Press **Open** next to **settings page**.
7. Set it up in the tab that opens.

## Two PC setup

One PC captures your input, the other draws the overlay. They talk over
your local network, so both machines need to be on it.

Start with the overlay PC. Set **Setup** to **Dual PC** and press
**receive**. Three things on that window are what you carry over:

- **this pc address**
- **port**
- **pairing key**

Then press **Start** and paste **browser source** into a Browser source in
OBS.

On the capturing PC, set **Setup** to **Dual PC** and press **send input**.
Fill those three into **overlay pc address**, **overlay pc port** and
**overlay pc key**, then press **Start**.

The overlay PC then says `linked to` and the other machine's name. Doesn't
matter which order you start them, they reconnect on their own.
