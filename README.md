# Bypass-LetterBoxing
### What is LetterBoxing?
A security anti-fingerprinting technique made by Mozilla to mask the actual screen dimensions of the device or browser window.
> The strategy here is to put all users in a couple of buckets to make it harder to single them out. 

> In simple words, this technique makes groups of users of certain screen sizes and this makes it harder to single out users on basis of screen size, as many users will have same screen size.

![](https://support.torproject.org/static/images/letterboxing.jpg)

###### More here
https://support.torproject.org/tbb/maximized-torbrowser-window/
https://www.zdnet.com/article/firefox-to-add-tor-browser-anti-fingerprinting-technique-called-letterboxing/
https://en.wikipedia.org/wiki/Letterboxing_(filming)
### Proof of concept
[Index.html](https://github.com/a7maadf/Bypass-LetterBoxing/blob/main/index.html "Index.html")
[Proof of concept video](https://vimeo.com/745627089 "Proof of concept video") // *Forgot to remove the video editing tool watermark lol*
### Risk
`low - medium`
- Although screensize dimensions might not be the only factor that compromises a Tor user's anonymity, they are a crucial piece of data that, when combined with other details, can be used to build a user profile.
- Because almost all other Tor users have similar screen sizes, people who fall victim to this vulnerability will be even more unique and easier to be targeted.
### Potential fix?
1. Disable all Javascript functions which manipulates the size of a browser's window.
2. Disable the LetterBoxing function from standard and safer modes.
3. Hmm, idk.
