# macOS Key Layouts for External Keyboards

A collection of English keylayout bundles for macOS to properly map keys on external keyboards.

## Install

1. Download the repository or any individual keylayout bundles.
2. Copy any relevant keylayout bundle(s) to `/Library/Keyboard Layouts`
3. Restart macOS
4. Open the input sources setup by going to **System Preferences > Keyboard > Input Sources**
5. Click on the [+] and select the installed bundle from the list to enable it.

At this stage you will have a Source Input option showing in the menu bar.

The Input Source menu will let you select the relevant input source once you connect the external keyboard. It will also let you quickly flip back to the default keyboard in macOS (for example, for me it would be _British_ for my UK MacBook Pro)

> If you don't want the entire bundle with included icon you could simply copy just the .keylayout file. You would then find it under an Others list in the Input Sources.

---

## Microsoft Designer Compact keyboard

The Microsoft Designer Compact keyboard bundle includes two keylayouts.

- **Designer Compact** - This is the standard UK PC layout as shown on the keys.
- **Designer Compact - ANSI Quotes** - This is similar to the UK PC layout except it switches the @ and " keys to be similar to US or all Mac keyboard layouts. Muscle memory is hard to break!

Here are the differences in table form.

| Key       | Designer Compact | Designer Compact - ANSI | Mac Keyboard |
| --------- | ---------------- | ----------------------- | ------------ |
| Shift + ' | @                | "                       | "            |
| Shift + 2 | "                | @                       | @            |

Furthermore, macOS swaps the `` ` `` and `\` keys on the Microsoft Designer Compact keyboard. Both of the provided keylayouts remaps the codes for these keys including all modifiers.

The bundle also includes a beautiful Microsoft logo.

### Install Microsoft Designer Compact keylayout

Open a terminal and run a sudo copy.

```
sudo cp -R Microsoft\ Designer\ Compact.bundle /Library/Keyboard\ Layouts
```

### Caveats

The Microsoft Designer Compact keyboard also has a lock button which triggers a `Win + L` keypress (or `CMD + L` in macOS). I couldn't find a way to override this to use the macOS lock sequence of `CMD + Ctrl + Q`.

You could create an All Application shortcut to use `CMD + L` within keyboard preferences. Click through to the _Shortcuts_ tab and select _App Shortcuts_ and add a new shortcut named **Lock Screen** with `Cmd + L` as the shortcut. Now macOS will lock when you press the corresponding Lock key on the Microsoft Designer Compact keyboard. This will conflict with Spotify's default Search shortcut though :/
