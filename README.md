# Scratch Font Userstyle

Code hosted for Scratch website userstyle that sets font to Fira Code. Works extremely well with Scratch Addons Website dark mode and customizable colors addons using the Dark WWW preset.

Gives the whole of the Scratch website an amazing monospace font called Fira Code, making your installation of [Scratch Addons](https://scratchaddons.com/) even better!

The userstyle requires access to [Google Fonts](https://fonts.google.com/specimen/Fira+Code) and only works on Scratch, but can work on other websites too. It's recommended to use this with the popular chrome extension/firefox addon [Scratch Addons](https://scratchaddons.com/)'s `Website dark mode and customizable colors` addons with the `Dark WWW` preset. Thanks to Stack Overflow for teaching me [how to import Google Fonts into a stylus file](https://stackoverflow.com/questions/25411486/how-to-import-google-fonts-on-a-stylus-file), I hit a big brick wall in learning that [I couldn't use the installed font with Chrome](https://github.com/openstyles/stylus/issues/793). 

## Intallation Instructions

- Get [Stylus](https://add0n.com/stylus.html) ([Chrome](https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne), [Firefox](https://addons.mozilla.org/en-US/firefox/addon/styl-us/), [Opera](https://addons.opera.com/en/extensions/details/stylus/))
- Install the [userstyle](https://userstyles.world/api/style/2432.user.css)
- Get [Scratch Addons](https://scratchaddons.com)
  - Enable `Website dark mode and customizable colors` addon
    - Use `Dark WWW` preset
- Go to [Scratch](https://scratch.mit.edu) and be happy.
  - Follow the [creator](https://scratch.mit.edu/users/-Xanimation-)

[![Screenshot](https://raw.githubusercontent.com/devxan/scratch-font-alteration/main/scratch-font-alteration.jpg)](https://scratch.mit.edu/users/-Xanimation-)

## Scratch Browser Extension/Userscript/Userstyle Policy
Browser extensions like Scratch Addons and Userstyles like the one mentioned above by @devxan are not allowed to be advertised on the Scratch website. This includes comments, within projects, and on the forums. You are still allowed to modify Scratch, but you aren't allowed to share with other Scratchers on the platform that you are doing so. More information about this policy is avialable [here](https://scratch.mit.edu/discuss/topic/284272).

## Modifying the Userscript
You can only really change the font. Do so by going to the [Google Fonts](https://fonts.google.com/) website, finding the font you want, selecting all styles (or a single one to make Scratch only use that specific font weight), and in the popup for the "Selected family" in the Use on the web section, select "@import" and copy the code between `<style>` and `</style>`. For Fira Code, that's:
```css 
@import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;400;500;600;700&display=swap');
```
Once copied, open up your browser extension for managing userstyles (for example, Stylus) and select the Scratch Font Alteration userstyle. Replace the code above with the code you got from Google Fonts. Then replace 
```css
font-family: 'Fira Code', monospace;
```
with the code under the header "CSS rules to specify families" on the Google Fonts website. Your final code should look similar to this:
```css
@import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@200;300;400;500;600;700&display=swap');

* {
    font-family: 'Fira Code', monospace;
}
``` 
But of course the mentions of the font I used are replaced with the font you use.

## Thanks
I really hope this small userstyle and repository might inspire you to learn more about modding Scratch and other sites with CSS and JS. I am really bad at both, so you can probably get a lot better than me pretty fast.
