# SCARTCouplers
This repo is a collection of SCART (EuroSCART) Gender changers/couplers, schematics, as well as some information I found difficult to find/understand when dealing with the SCART standard.

*completed pcb images*

# Why/About

When I was designing a [previous project](https://github.com/circuitsable/SCARTAudioExtractor), I had to fully understand the SCART standard for the project to be sucessful, which I found difficult to do. This may be due to my inexperience in dealing with connectors or understanding concepts of how the video signals being sent over the SCART cable work. This repository includes working schematics & PCBS for SCART gender changers/couplers, as well as a very short "cable", which would have helped me greatly when desinging my previous project.

I am hoping this information may be helpful to someone else, despite how easy this may be to figure out on your own or its nicheness.

# Info

The [wikipedia page](https://en.wikipedia.org/wiki/SCART) on SCART says much more than I could and in a more concise manner. The standard documentation for SCART is still available for purchase, but can be found online as a [scanned document](http://fr.meric.free.fr/Articles/articlesba/stsurtvplat/Scart/BS_EN_50049-1%20Peritelevision%20connector.pdf).

## "Input" & "Output"

Looking at the pinout of the connector on wikipedia, there are pins labeled as input and output for the daisychainability of the connector and its signals. This caused me much confusion, as I was unsure if input meant that the signal traveling across the cable was an input to another device, or was the input from the previous device. Input is where you are meant to take in input, from the previous device. 

## Impedance matching

High frequency signals, including video signals, may have the traces they run along have a matching impedance to improve reliability of the signal. When dealing with the average signals sent over a SCART connection (cable or PCB traces, 240p/288p/480i/576i), this is not a concern.

## Grounding

It is okay to join most or all of the grounds together, including the shell. In theory the seperate grounds can help with the integrity of the signals, but in practice it is just fine.

## Termination

Termination (parallel or series) is only done at signal transmitters (e.g. game console) and signal recievers (e.g. television). Your cable/gender changer should ideally be 2 ports and connections between them, nothing else.

## Audio

The audio signal on a SCART cable is perfectly fine to tap into and use for more common audio connectors, such as a 3.5mm audio jack or RCA/phono jacks. The signal wont be too loud or anything like that

# PCB Images & Schematics

*images*
