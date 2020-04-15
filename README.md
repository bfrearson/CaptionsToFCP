# LyricsToFTP
Automator script in JXA to generate a captions file.

##**Note**
This is a *very* early release—I've not put any validation or error checking in here. I'm happy to help debug any issues, but expect things to break if you try anything weird

## **Introduction**
This package will install a service that can run on any text selection and generate a series of 10 second captions for Final Cut Pro for every pair of lines of text. The file is output to ~/Movies/CaptionsToFCP


## **Installation**
Running the installer will install the following files:

~/Library/Application Support/CaptionsToFCP/FCPCaptionsBlank.itt <-- template file that the script modifies

~/Library/Services/Generate Captions for Final Cut Pro.workflow <--Automator workflow containing Javascript for Automation script


## **Usage**
With any text selected, right click -> Services -> Generate Captions for Final Cut Pro.

Note: The first line of text will be used as the title and will not appear in the timeline in Final Cut Pro.

A single line break moves text to the next line. A double line break indicates the start of a new caption.


My typical usage is to copy a script into a Note or Textedit file, and format by adding new lines after the title.

When the script is executed, a new file will be placed in ~/Movies/CaptionsToFCP

### **Sample Lyrics**
This is what the script expects to see:

```
Genesis 1

In the beginning God created the heavens and the earth.

Now the earth was formless and empty,
darkness was over the surface of the deep,
and the Spirit of God was hovering over the waters.

And God said, “Let there be light,”
and there was light.

God saw that the light was good,
and he separated the light from the darkness.

God called the light “day,” and the darkness he called “night.”

And there was evening, and there was morning—the first day.
```


This is an extension of [Lyrics to FCP](https://github.com/bfrearson/LyricsToFCP) which generates lyrics overlays with more customisability than captions offer.  I hope it blesses your church.

Ben Frearson
