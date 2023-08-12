# Sound/image media files have gone missing!

Anki stores your cards' sound and image files on your computer, in your [Anki folder](https://docs.ankiweb.net/files.html#file-locations), in User 1/collection.media. If you delete any files from that folder, Anki notes they have been removed and on the next sync it will remove them from your other devices as well. What sometimes happens is users tidy up files on their computer, and accidentally remove the sounds and images that their cards use, resulting in sounds not playing or images not appearing. This is particularly easy to do accidentally on a Mac with the "all my files" feature of the Finder, but can happen on other platforms as well.

You can use Anki's Tools>Check Media function to find out which images are missing from your collection by looking at the "Used on cards but missing from media folder" section.

If you've accidentally deleted the files your cards were using, you may be able to restore them from your recycle bin / trash can if the trash has not been emptied yet. Placing them back in the collection.media folder should cause the media to work again.

If you are unable to recover your media from any of your devices, we may be able to restore it from AnkiWeb's backups for you if it was deleted recently.

If you've lost your sound and images, but had obtained them from a shared deck, if the shared deck is still available you can import it into a new profile, and then copy the sounds and images from it into your original collection to restore the data.

When editing fields, Anki shows the names of sound files. To see the names of image files, you can press ctrl+shift+x while the cursor is in the field with the image (cmd+shift+x on a Mac). For an image or sound file to work, a file with the exact same file name must be in the collection.media folder.
