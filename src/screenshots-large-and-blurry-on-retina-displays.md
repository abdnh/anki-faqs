# Screenshots large and blurry on retina displays

If you edit a card, click on Cards, and then place the following at the very
bottom of the styling section, it will shrink screenshots down to the correct
size:

```
img[src*="Screen"] { 
  zoom: 50%;
}
```

It works by targeting any filenames that have "Screen" in them - which applies
to the default "Screen Shot" name that macOS uses. If your screenshots use a
different but consistent name, you can adjust the line above.

If your screenshots use names that don't have a consistent pattern, you can
remove the square brackets and the text inside them, which will cause all images
to be matched. Images from high resolution displays will now look correct, but
images you obtain from other sources may now look too small. Unfortunately there
is no good solution to this problem at the moment - the web technologies Anki
uses do not have a way of detecting which images need to be resized. Resizing
the images prior to adding them to Anki will allow you to mix and match other
images, but it requires some setup:
<https://www.quora.com/How-can-I-get-my-retina-Mac-to-not-take-screenshots-that-are-too-big>

If you're on Windows, an Anki user suggested using SnagIt as a workaround:
<https://anki.tenderapp.com/discussions/ankidesktop/38152-feature-request-de-zoom-picture-pasted-with-a-certain-hotkey>
