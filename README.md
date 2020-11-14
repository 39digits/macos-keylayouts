# MacOS Key Layouts for External Keyboards

A collection of English keylayout bundles for MacOS to properly map keys on external keyboards.

## Install

1. Download the repository or any individual keylayout bundles.
2. Copy any relevant keylayout bundle(s) to `/Library/Keyboard Layouts`
3. Restart MacOS
4. Open the input sources setup by going to **System Preferences > Keyboard > Input Sources**
5. Click on the [+] and select the installed bundle from the list to enable it.

At this stage you will have a Source Input option showing in the menu bar.

The Input Source menu will let you select the relevant input source once you connect the external keyboard. It will also let you quickly flip back to the default keyboard in MacOS (for example, for me it would be _British_ for my UK MacBook Pro)

> If you don't want the entire bundle with included icon you could simply copy just the .keylayout file. You would then find it under an Others list in the Input Sources.

## Microsoft Designer Compact keyboard

The Microsoft Designer Compact keyboard is your standard UK PC layout, however MacOS swaps the `` ` `` and `\` keys on this keyboard. This keylayout bundle simply remaps the codes for these keys including all modifiers and includes a beautiful Microsoft logo.

### Install Microsoft Designer Compact keylayout

Open a terminal and run a sudo copy.

```
sudo cp -R Microsoft\ Designer\ Compact.bundle /Library/Keyboard\ Layouts
```

### Recommended Settings

The Microsoft Designer Compact keyboard also has a lock button which triggers a `Win + L` keypress. I couldn't find a way to override this so I usually add a custom lock shortcut in MacOS instead.

Open Keyboard preferences and click through to the _Shortcuts_ tab. Click on _App Shortcuts_ and add a new shortcut named **Lock Screen** with `Cmd + L` as the shortcut.

Now MacOS will lock when you press the corresponding Lock key.
