This is a irssi script to automatically issue bitlbee `rename`
commands for nonsensical nicks like `u1359078110`, changing them into
e.g. `AEvarArnfjord`.

To do this it uses the
[Text::Unidecode](http://search.cpan.org/perldoc?Text::Unidecode)
module. You must install it for the script to work, either from CPAN
or from your package manager. E.g. `aptitude install
libtext-unidecode-perl` in Debian and Ubuntu.

Additionally, Bitlbee itself must be configured to use `utf-8` as its
`charset`. To find out if that's the case, do this in the `&bitlbee`
channel:

    <@avar> set charset
    <@root> charset = `utf-8'
    
If not, just set the charset to `utf-8` like so:

    <@avar> set charset utf-8
    <@root> charset = `utf-8'

# Author

This script is originally from
[nowhere.dk](http://www.nowhere.dk/articles/facebook-chat-in-bitlbee)
modified by Ævar Arnfjörð Bjarmason to support Unicode names.
