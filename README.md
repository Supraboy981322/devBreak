# devBreak
**A simple _stylized_ web based web development client using [webssh](https://github.com/huashengdun/webssh/) with a preview.**

---
## Note:

This has only been tested with [Apache](https://httpd.apache.org/) and [webssh](https://github.com/huashengdun/webssh/), therefore, I cannot guarantee that it'll work with alternatives. **Please do not submit an issue if you are not using Apache and webssh.**

---
## Shortcuts

- [Note](#note)
- [Installation](#installation)
- [Interface](#interface)
- [Usage](#usage)
- [Customization](#customization)

---
## Interface

Login screen:
![Not connected screenshot](/img/logged-out.png)

Connected:
![Connected screenshot](/img/connected.png)

---
## Installation
>**Before you begin, you must have [webssh](https://github.com/huashengdun/webssh/) and [apache](https://httpd.apache.org/) already installed on your server.**

- First, download the [latest release](https://github.com/Supraboy981322/devBreak/releases) `.7z`, `.zip`, or `.tar.xz` (this tutorial will assume you chose `.tar.xz`, adjust the file type in the link for your format)

  `sudo wget https://github.com/Supraboy981322/devBreak/releases/download/[latest release]/devBreak.tar.xz`

- Then, extract it (again, this tutorial will assume you picked `.tar.xz`, so adjust the command for your format)

  `tar -xf devBreak.tar.gx`

- Next, move it to the directory of your choosing on your web server.

  `mv devBreak [location of your directory]`

- Open `index.html` in your text editor (this tutorial will assume `nano`. 

  `sudo nano [location of your directory]/devBreak/index.html`

- Modify the `src` tag under the iframe after the corresponding comment with your webssh client URL.

  `<iframe class="frame" id="devEnvironmentFrame" src="[Your webssh URL]"></iframe>`
  
---
## Usage

### The webssh frame:

Once the page is setup, it is farly easy to SSH into your server. 

- Sign-in:
  * Enter the *hostname* or *IP address* of your SSH server
  * Enter your *username*, *password*, *private key*\*, *passphrase*\*, and *TOTP*\*
    >Private key, passphrase, and TOTP are optional
- Use the application of your choice for web development
  > I recommend GNU nano (`sudo nano`), or Vim, I tested (only because I tested both and GNU nano is included in most major Linux distributions)
- Alternatively, you could enter the URL of the site of your choice into the *address bar* directly above the frame

### The preview frame:

By default, the preview frame does not display anything on load. However, you can set the default URL for the preview frame when the web page is loaded:

- Just like setting the webssh URL, in the file titled `index.html`, add the URL to your webpage in the `src` tag in the iframe under the corresponding comment.
  
  `<iframe class="frame" id="previewFrame" src=""></iframe>`

Alternatively, you could enter the URL to your preview page each time you the load or reload devBreak.

  - Just above the preview frame, enter the URL to your preview page in the address bar and press the "***Go***"  button located immediately to the right of the address bar.

As of now, the preview frame does not refresh automatically, so you must manually refresh the page.

  - Above the preview frame, to the right of the "***Go***" button, press the button labled "***&#x27F3;***" to refresh the preview frame.

---
## Customization

By design, devBreak is highly customizable. Using custom CSS and a background images, you can make devBreak look as unique or stylistic as you please.

>Please note: in order to make custom styling, you must have at least novice to moderate knowledge of CSS.

Every element of devBreak was designed to be modified to your liking. Even webssh can be customized (see the documentation on [the webssh GitHub page](https://github.com/huashengdun/webssh/) for information/instructions)

### Examples:

["tbd" - by tdb](tbd)
![tbd](https://supraboy981322.github.io/uncanny%20gobledygook.png)

["tbd" - by tbd](tbd)
![tbd](https://supraboy981322.github.io/uncanny%20gobledygook.png)
