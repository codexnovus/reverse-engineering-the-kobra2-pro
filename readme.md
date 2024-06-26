# Reverse engineering the Kobra 2 Pro

_**Note:** this probably is also applicable to Kobra 2 Plus and Max, as they seem to use the same motherboard and printhead, but I do not own one of these, so I cannot confirm_

The purpose of this repository is sharing my efforts to make the new Kobra 2 Pro machines usable. Suffice to say, I'm very dissatisfied with Anycubic's decision to block serial input and force us to print through their servers - and accepting terms that include giving anycubic the rights to reproduce anything we upload to our printers, and the right of anycubic to disconnect our printer if they feel we are doing **illegal things**, without very much specifics about what they consider illegal.

Anyway, I could rant over how they have not published the source code, which probably is a violation of the GPL, as a cursory examination of the files show klipper headers over there, or how I feel about them ommitting the fact that we no longer have direct control on our printer.

Instead of that, let's just go over what I found so far.

* [The Motherboard](./motherboard/index.md): I've successfully identified all pinouts. Over on Klipper forums they posted how to use the serial connection to enable access to the underlying linux system.
* [The Printhead](./printhead/index.md): I'm 99% sure I have the correct pinout, but I still need to correctly identify the accelerometer IC in order to verify the correct SPI pin assignment.
* [The Bed](./bed/index.md): Pinout and components identified.


## Other noteworthy efforst I've saw, and references:
* The thread that started it all: [Printer.cfg for Anycubic Kobra 2 Plus/Pro/Max](https://klipper.discourse.group/t/printer-cfg-for-anycubic-kobra-2-plus-pro-max/)
* Referenced on the thread, user _kenguru_ has released a modification that allows you to redirect the MQTT messages to a server of your own, bypassing the need of using the anycubic app. [Kobra unleashed](https://github.com/anjomro/kobra-unleashed)
* User [1coderookie](https://github.com/1coderookie) is compiling information about the Anycubic Kobra 2 Pro on his [Kobra2Pro Insights Page](https://1coderookie.github.io/Kobra2ProInsights/)
* Anycubic Reddit community has published a [FAQ for Kobra 2 Series](https://www.reddit.com/r/anycubic/comments/19113t3/faq_for_kobra_2_series/) that summarizes many of the main points of the conversation.


---
Feel free to use any of the information I collected, including schematics and technical data, on your projects. Attribution by name would be appreciated, linkback not needed.

<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/codexnovus/reverse-engineering-the-kobra2-pro">Reverse Engineering the Kobra 2 Pro</a> by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://github.com/codexnovus/">codexnovus</a> is licensed under <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"></a></p>
