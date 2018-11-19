# nightcrawler
project to build an imaging app for low key surveillance

## parts list
Raspberry Pi Zero Wireless - Starter Kit
Raspberry Pi NoIR Camera - 8 Megapixel (V2)
Raspberry Pi Zero Camera Cable
Electrical Tape

## overview
I think there's activity in my backyard at night. This is not unusual because I live in a fairly rural area and there is
no shortage of wildlife, like raccoons and deer. This is a home project I'm undertaking to put together a low key
surveillance system for under $100 to see what's going on. It intends to:

1. Use the Raspberry Pi NoIR Camera to take pictures.
2. Send those pictures to a storage repository.
3. Process those pictures

# Requirements

1. Taking Pictures
* When the camera notices movement, start taking pictures at configurable intervals
* after movement ends, slow down the intervals for a configurable amount of time then stop filming
2. Storing Pictures
* Store in a web-accessible repository, probably Dropbox to start
* Structure the repository in a Year, Month, Day, Event Time structure
3. Process Pictures
* Apply some sweet algorithms like:
    * Face detector
    * Object classifier
* send a notification
* When new pictures are uploaded, send a notification when specific criteria are met

#Architecture
[pi] -> [Drop box] <- [web app]


# Pi Applications required:
* https://github.com/andreafabrizi/Dropbox-Uploader

# Web App Libraries required:
* https://www.pythonforbeginners.com/code-snippets-source-code/using-python-to-send-email/



