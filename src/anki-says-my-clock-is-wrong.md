# Anki says my clock is wrong

To ensure your scheduling doesn't get messed up, Anki requires that your device's clock is set correctly. This means all of the following must be set correctly:

- the time (including AM/PM)
- the date
- the timezone
- daylight savings

If you receive an error about the clock being wrong, please check to ensure all of the above are set correctly. Please note that even if your system is showing you what looks like the correct time, if the above settings are not correct, the computer's internal idea of the correct time may be wrong.

**"What should I do if my country has just changed its handling of daylight savings?"**

When politicians change the handling of daylight savings time, it can take companies like Windows and Apple time to update their operating systems to reflect the new handling. To work around the problem, you can select a different timezone that has the same UTC offset as your current location, and then update the clock to make sure it is correct. For example:

- it's 10AM where you are
- you've checked Google for the current standard time, and it's currently midnight: <https://www.google.com/search?q=utc+time>
- this means you are ten hours ahead of standard time, so your UTC offset is +10:00
- in your system settings, look for a timezone that is +10:00
- after adjusting the time zone, adjust the clock so it shows the correct time

**"Why doesn't Anki let me ignore the error?"**

If you study while the clock is incorrect, then your progress is likely to be messed up when any of the following happen:

- the clock is automatically reset to the correct time in an OS upgrade
- you decide to start using AnkiWeb for backups or deck sharing
- you decide to start studying on multiple devices
- you move to a new machine after the old one breaks
- you manually change the time because other apps also notice the clock is wrong

Anki refuses to start up because an incorrect clock will also cause issues like file modification times to be wrong, and it's better to address the issue than hide it away and risk issues in the future.
