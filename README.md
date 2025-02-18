# Open Android Radio Station Lists
In this document are a variety of JSON files, these correspond to station presets I have created which are used as the default import options in [Open Android Radio](https://github.com/TypicalNerds/Open-Android-Radio).

# Are these stations Geo-Restricted?
Most of these stations will be using URLs tailored for UK Audiences, this means that they may not be supported or may be geo-restricted for users outside of the UK.
These URLs may break or change without warning so don't rely on them as your primary reliance.

# Where do you source these links?
Radio Stream that are provided here are licensed with permission directly from radio operators, this means not all stations are included.

If any radio operators want their stations removed, please contact me or submit a takedown notice with the name of your company and all associated stations that I can confirm are related to your company will be removed, provided that the notice comes from an organisational email address (not just a generic personal gmail account).

# How do you get the logos?
Logos are grabbed from various sources such as google and extracted from webpages of stations, and are then modified to fit a more ideal aspect ratio to improve visiblity.

If you wish, take a look at my [Logos Repo](https://github.com/TypicalNerds/LakesideTV-Channel-Logos) where many of the links in these presets will point to. 

# FAQ for Radio Station Operators
## Can you forcefully remove stations from user's devices?
As of writing, no, this is because removing stations from presets only prevents users from adding it again in the future using the app's built-in station import function.
There are also a couple of other reasons this isn't feasible.
- Attempting to write something to detect unauthorised station urls and removing them requires embedding the detecting in a full app update, which is more likely to wipe out entire configs than just a single station.
- This goes against the point of the app, the app is meant to be open, and as the code is open-source, anyone can just create a fork and remove the detection measures themselves.
- The app already uses a custom user agent, which would just be easier for you to block yourself, but remember, anyone can re-write the code themselves to bypass this.

## Do you have any means of geo-restricting your stations?
No, I do not have any means to geo-restrict content within my technical skills, other than by offering a means for the user to choose their country, but this is flawed because it could easily bypassed anyways through modifying the code or just by saying they are in another country.
The best way to approach this is to geo-restrict by IP address and sending users outside your desired region a audio message telling them they have been blocked due to their location.
One example of a company that does this is Audacy, who use geo-restrictions to restrict their stations to within the United States, attempting to listen outside the USA gives you a piece of audio that tells you the station is not available in your country, alongside instructions on how to resolve the issue if your within the United States.

## Can I host my own presets?
At the moment, as of v0.0.7-beta, I don't have a means of adding country selection at the moment, but theoretically, if I did some work to add it, then you absolutely could.
Please note you would need to create your own presets for the regions you operate in and for your country, from there, ask me to add your configuration url to the config file which is used by the OAR App to locate presets and from there, all you'd be responsible for is keeping the files online, publicly available and up to date.
