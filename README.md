# devBreak
**A simple _stylized_ web based web development client using [webssh](https://github.com/huashengdun/webssh/) with a preview.**

---
## Note:

This has only been tested with [Apache](https://httpd.apache.org/) and [webssh](https://github.com/huashengdun/webssh/), therefore, I cannot guarantee that it'll work with alternatives. **Please do not submit an issue if you are not using Apache and webssh.**

---
## Shortcuts

- [Note](https://github.com/Supraboy981322/devBreak/#note)
- [Installation](https://github.com/Supraboy981322/devBreak/#installation)
- [Interface](https://github.com/Supraboy981322/devBreak/#interface)


## Interface

Login screen:
![Not connected screenshot](/img/logged-out.png)

Connected:
![Connected screenshot](/img/connected.png)

---
## Installation
>**Before you begin, you must have [webssh](https://github.com/huashengdun/webssh/) and [apache](https://httpd.apache.org/) already installed on your server.**

- First, download the [latest release](https://github.com/Supraboy981322/devBreak/releases) `.7z`, `.tar.gx`, or `.tar.xz`

- Then, extract it

- Next, move it to the directory of your choosing on your web server.

- Finally, run `sudo nano [file path of index.html for devBreak]` and modify the `src` tag under the iframe after the comment with your webssh client URL.