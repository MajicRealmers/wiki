---
title: Set Command Prompt
type: docs
prev: manual/death
next: locations/
---

Your prompt is a powerful tool to display current status. The limit on length is 30 characters and you can use the following special character strings:

- `%c#` Foreground color (0 = black, 1 = red, 2 = green, 3 = yellow, ...)
- `%b#` Background color (4 = blue, 5 = violet, 6 = cyan, 7 = white, ...)
- `(r` = reset (to your terminal's default)
- `%k` Target's name  
- `%l` Target's condition  
- `%m` Default Target String
- `%n` Tank's name  
- `%o` Tank's condition  
- `%p` Default Tank String
- `%h` Current hit points  
- `%i` Max hit points  
- `%j` Percentage HP
- `%s` Current spell points  
- `%t` Max spell points  
- `%u` Percentage SP
- `%x` Current experience  
- `%y` Exp for next level  
- `%z` Exp remaining
- `%%` Displays a '%'  
- `%f` Bank Gold  
- `%g` Gold on hand
- `%e` Default Exit String  
- `%d` Raw exits string

For example the default prompt is set as: (without the quotes)

`HP=%h SP=%s%cr%br>`

Note that some default colors are set before prompt printing starts, so if you change the colors your prompt will not be highlighted if your health is low. You can also enter just a '!' to have your prompt set to the default or a blank line to abort. If you enter just a '1', '2' or '3' you will be given one of our sample prompts.

**Old Prompt:** `'%j hps %z xp needed %d exits'`

If using Mudlet, you can then set your mapper configuration using something like:

`map prompt H:%d S:%d X:%d T:%s>`

If you are not seeing your prompt, the status line may not be enabled. To enable, use the command:

`statline``
