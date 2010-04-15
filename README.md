This is a irssi script to automatically issue bitlbee `rename`
commands for nonsensical nicks like `u1359078110`, changing them into
e.g. `AEvarArnfjord`.

It supports nicks in the Unicode range via
[Text::Unidecode](http://search.cpan.org/perldoc?Text::Unidecode).

# Author

This script is originally from
[nowhere.dk](http://www.nowhere.dk/articles/facebook-chat-in-bitlbee)
modified by Ævar Arnfjörð Bjarmason to support Unicode names.
