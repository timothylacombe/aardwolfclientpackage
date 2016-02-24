Description:

The VI_captures plugin constructs what we will call "captures". 
Captures let you assign a keyword to some text, timestamp it, and store it sequentially with all other stored text of the same keyword.
You can then call up a particular keyword and navigate through the stored messages for that keyword using built-in commands.
You also get a command to copy the currently navigated message to your computer's clipboard.

This plugin will also automatically detect URLs in stored messages as long as they start with either http:// or https://.
Recalling a stored message that has detected URLs will notify you how many URLs were detected and allow you to cycle through them, copy them to your computer's clipboard, or open them directly in your computer's default web browser.

This plugin also lets you define whether you want particular storage keywords to be automatically spoken aloud at the moment of storage.
If URLs are detected, you will be notified then too. There is a special command for jumping directly in the captures navigation tree to the message with the most recent automatically spoken batch of URLs.

Commands:

All commands for this plugin start with the two words "mush capture". You can of course create your own redirecting accelerators or aliases to remap these for convenience, but this keeps the commands in their own logical namespace.

The commands are as follows...

mush capture switch
This command takes the mandatory argument of an existing capture keyword and points future message navigation commands at the given keyword's batch of messages.

mush capture next
mush capture prev
These two commands step through the captures instead of having to remember the keywords.

mush capture list
This command takes an optional argument of either loud, quiet, history, or nohistory, and lists all of the captures with the given flag. If no flag is given, then it lists all known captures.

mush capture next line
mush capture prev line
mush capture first line
mush capture last line
These four commands step through the captured messages of the currently navigated capture keyword.

mush capture show
This command shows the currently navigated captured message.

mush capture copy
This command copies the currently navigated captured message to the operating system clipboard.

mush capture copy next url
mush capture copy prev url
These two commands step through the detected URLs for the current navigated message and copy the current one to the operating system clipboard.

mush capture browser copied url
This command takes the current URL from the previous commands and opens it in your operating system default web browser.

mush capture delete line
This command permanently removes the currently navigated message from the capture buffers.

mush capture clear
This command permanently removes all messages from the currently navigated capture buffer.

mush capture remove
This command gets an optional argument and removes either the current or given capture keyword and all of its stored messages.

mush capture loud
This command gets an optional argument and sets either the current or given capture keyword to automatically speak messages when storing them.

mush capture quiet
This command gets an optional argument and sets either the current or given capture keyword to not automatically speak messages when storing them.
