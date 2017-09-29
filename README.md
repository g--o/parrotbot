# ParrotBot
ParrotBot is a simple Discord bot solving a simple Discord problem: That it
doesn’t support quotation.

## Usage
With ParrotBot, you can easily quote other messages, as long as they are in the
same channel and weren’t posted too long ago.¹ Just send a message containing
a greater-sign (>), followed by an excerpt from the message you want to quote –
just like many people do anyways. ParrotBot will automatically find the most
recent occurrence of this quote, display the according message in a box, and
delete the text-only quote you sent (if you allow it to):

![Example quote](https://github.com/mart-w/parrotbot/blob/master/doc_img/example_quote.png?raw=true)

![Example result](https://github.com/mart-w/parrotbot/blob/master/doc_img/example_quote_result.png?raw=true)

“But what if there are multiple similar messages from different users and it’s
not the last one I want to quote,” I hear you ask? Well, in this case, you can
just put the user name, nickname or user ID of the author in front of the
greater-sign and clever little ParrotBot will only consider messages from that
user.


¹ To reduce server load, the number of messages searched is limited. That limit
can be adjusted to your needs, of course.

## Installation
To run ParrotBot on your machine, you need Python 3.5 or higher and
[discord.py](https://github.com/Rapptz/discord.py) v0.15.0 or higher.
ParrotBot also uses the modules `asyncio`, `datetime`, and `re`, but those
should normally already be part of your Python installation. You also need a
Discord bot user and its API token (see https://discordapp.com/developers for
further information on that).

If you have all that, just clone this repository and create a file called
`token.txt` in the repository’s root folder containing nothing but the API
token. Then you’re ready to go! Insert your bot’s client ID into this URL:

    https://discordapp.com/oauth2/authorize?client_id=YOUR_ID_HERE&scope=bot

Open it, choose the server you want to add your bot to and click on “Authorize”.
Then the only thing left to do is to fire up `parrotbot.py` and quote away!

## Contribution
If you find a bug or want to suggest a new feature, feel free to create a new
issue here on GitHub, I will look into it.

If you feel like contributing to the codebase itself, that is also appreciated!
Just fork the project, make your changes and file a pull request that describes
what you’ve done. Please try to write clean, understandable code and document it
as described in
[Python’s docstring conventions](https://www.python.org/dev/peps/pep-0257/#specification).

Whatever you do: Please stay polite and friendly. We’re all doing this for fun.
:wink:

## License notice
Copyright (C) 2017  Martin W.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
`LICENSE` file or http://www.gnu.org/licenses/ for details.
