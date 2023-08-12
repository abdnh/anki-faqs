# Shared decks with broken Javascript

Some shared decks make use of a feature called 'Javascript', which allows them to dynamically modify the display of the card. Javascript can be fragile, which is why the Anki manual recommends deck authors avoid it. It may break when Anki is updated, or when the deck author has not tested their Javascript on the different Anki platforms.

If you encounter a Javascript error in a shared deck, please post a review on the shared deck download page to let the deck author and other users know of the problem. If the deck author is active, they will hopefully address
the issue in a future update.

If the deck author is unable to help you, you can try edit your card template to remove the Javascript to prevent an error from showing. Depending on what the Javascript was doing, this may result in lost functionality.

To do so, using the computer version of Anki:

- Use File>Export to export your entire collection with scheduling information. This will give you a backup that you can restore to if anything goes wrong.
- Edit a card, and click the Cards... button.
- Look for areas in the front and back template that start with `<script>` and end with `</script>`. Remove the start and end, and everything in between.
- Confirm that the card displays in the review screen without error. If it's working ok, you can sync your changes to AnkiWeb and then to your other devices.
- If removing the script has completely broken the card, use File>Import to restore to the backup you created.
