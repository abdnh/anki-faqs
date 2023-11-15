# "Some updates were ignored because note type has changed"

When importing a shared deck that has previously been imported, Anki will only be able to update your existing cards if:

- the name, number and order of fields has not changed
- the name, number and order of card templates has not changed

Changes to the front and back template will not prevent updates.

If changes have been made to the fields or card templates and you want to apply updates, you will need to modify the note type in your collection to match the one in the deck you're trying to import. To do this, you can import the shared deck into a new profile, note down the note type's fields and card templates, and then compare them with the note type in your profile.

If you're not concerned with updates, and just want to grab any new cards, one way to make importing work is to delete the old note type via the Tools>Manage Note Types screen. This will delete any cards associated with it, so if you wish to preserve the existing cards, you'll need to manually use the Change Note Type option in the browse screen to move them to a new note type.

Please note that if the deck sharer has used the 'change note type' option in their collection, they will have permanently broken link between your copy and theirs, and updating via .apkg import will not be possible even if your note type's fields and card templates match. You can check the note types are linked by using the following command in the [debug console](https://docs.ankiweb.net/misc.html#debug-console) while looking at a card in the study screen:

```
pp(card()['_note'].mid)
```

Repeat for the shared deck imported into a temporary profile. If the numbers match, the note types are still linked.

If one of the fields in the shared deck has not been altered, it is also possible to apply updates via a text import. After importing the shared deck into a temporary profile, use File>Export to save the notes in txt format. Then in your original profile, you can import the text file, matching against a field that has not changed. Text imports can only operate on one note type at once, so if the shared deck you've downloaded contains multiple note types, you'll need to do the process one note type at a time. More info is at <https://docs.ankiweb.net/importing/packaged-decks.html#updating>.
