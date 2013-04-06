alfred-date-calculator
======================

Alfred workflow to display or calculate with current date and time.

Usage
-----

Install workflow and enter `date` to get the current date as a search result. Pressing enter will copy the formatted date to clipboard.

![Date Calculator in Alfred](https://raw.github.com/LeEnno/alfred-date-calculator/master/screenshot_date.png)

You can add or subtract years, months, weeks, days, hours, minutes and seconds i.e. to calculate a date in the future. Refer to the chapter *Options*.

Options
-------

You can use:

- **y** for *years*
- **m** for *months*
- **w** for *weeks*
- **d** for *days*
- **h** for *hours*
- **min** for *minutes* (not colliding with **m** for months)
- **s** for *seconds*

Prepend a number to the identifiers and optionally a minus sign for subtracting.

**Examples:**

- `date 3w`: today + 3 weeks
- `date -2y`: today - 2 years
- `date 2m -5d`: today + 2 months - 5 days

Change Default Format
---------------------

You Probably don't want to stick with the default date format. Changing it is pretty easy. Just enter `dateformat` and type the format you like (or choose from the suggestions). You have to give a string as used in <s>[PHP's `date` function](http://php.net/manual/en/function.date.php "PHP date")</s> [strftime](http://strfti.me/ "strfti.me: strftime reference and sandbox for Ruby, Python, PHP"). You can disregard the `%`-character. The script will add it automagically for you.

Preview will be shown in realtime.

![Date Calculator in Alfred](https://raw.github.com/LeEnno/alfred-date-calculator/master/screenshot_dateformat_simple.png)

![Date Calculator with custom format](https://raw.github.com/LeEnno/alfred-date-calculator/master/screenshot_dateformat_custom.png)