## Data formats

### Date & time
1. These guidelines apply to US English content only.
2. The following formats are covered in this section:
  1. Current date and time
  2. Date and time settings (such as an alarm or reminder)
  3. Date and time events (such as when an object was created, sent, edited, or otherwise acted upon)
3. Date and time
  1. Time
    1. If a timestamp is within the current day, display the time using uppercase AM or PM, without periods:
    2. hour:minute AM/PM
  2. Month and day
    1. If within the current calendar year, display the date without the year.
  3. Month, day, and year
    1. If not within the current calendar year, display the date and year.
  4. Abbreviations
    1. Abbreviations are fine in English.
4. Time and date ranges
  1. En dash
    1. Separate a range of dates or times with an en dash, without spaces. When spelling out months, or to remove ambiguity, add spaces around ranges.
  2. Year
    1. Unless both dates in a range start and end in the current year, show the year on both the start and end. Date/time libraries often show a range within the same month.
  3. Common AM/PM
    1. When a range shares a common AM/PM, append once at the end of the range.
5. Time zones
  1. When listing the time zone, drop the leading 0 for single digits.
  2. Single times zones
    1. Remove the S (for Standard) or D (for Daylight) for specific time zones (EST, EDT).
  3. Combined time zones
    1. When specifying a date for a nationwide audience, include Standard or Daylight acronyms (such as EDT) to avoid confusion. This is because some U.S. states, such as Arizona, don't use daylight savings time.
6. Human and relative language
  1. Display date and time information as people normally speak to each other, when space permits.
  2. Refer to yesterday or tomorrow in those terms.
  3. If the day is in the future and within a week, display the day of the week.
  4. Display word alternatives that help understanding or describe a time-of-day.
7. Approximate time
  1. If absolute time isn’t necessary, you may display approximate times, rounding down to the most recent largest unit.
  2. When relative language isn’t appropriate, use absolute time. Absolute time includes the specific time of an event or the time appearing on a clock.
8. Context adjustments
  1. Depending on the context, show either date or time, or both date and time.
  2. Future
    1. Append time to a future day or date.
  3. Past
    1. When a past time is necessary, display both date and time.
  4. Weekday
    1. When the day of week is necessary, display the abbreviated day separated by a comma. For instance, calendar invites should display the day of the week and the date and time.
  5. Distant past
    1. Omit the time for events in the distant past.
  6. Duration
    1. Show the duration of a recording, like audio or video, in this format:
    2. H:MM:SS
    3. Omit hours or seconds if they don’t apply.
    4. To avoid confusion, use the same format should across the same context. For example, if one video uses 3:15 to mean 3 hours and 15 minutes, another video on the same page should not use 3:15 to mean 3 minutes, 15 seconds.
9. Abbreviations
  1. Where real estate is limited, use abbreviations for months and days.
  2. Months can be abbreviated or numeric.
  3. Days of the week can be abbreviated using the first letter of each day. (S for Sunday, M for Monday, etc). Single-letter abbreviations can be ambiguous, so the context must clarify the meaning.
  4. Abbreviated days of the week can be combined with a time.
  5. Abbreviate units, or numerical versions, by removing the “:00.” Abbreviated units are appropriate for timestamps, labels on graphs, durations, etc.
10. Other languages
  1. Many non-English languages use lowercase am and pm.
  2. Many languages do not abbreviate month names.
  3. Abbreviations are fine in English, as long as they don't disrupt translations that require the full name. In many languages, there are no abbreviations for month names.
  4. In US English, the en dash does not have spaces before or after it.
  
### Data redaction and truncation
1. Data redaction with midline ellipses
  1. Midline ellipses [• • •] are three-bullet glyphs used to represent numeric truncation and the redaction of sensitive data, such as credit card, debit card, and Social Security numbers.
  2. Midline ellipses preserve user security by mimicking masking, effectively punctuate numerals not shown, and reflect the vertical midline symmetry of material design.
  3. Usage
    1. Before the first midline ellipse, place two regular spaces, then add a thin space between each midline ellipse and after the final midline ellipse. Or, use the unicode string: U0020,U0020,U2022,U2006,U2022,U2006,U2022,U2006
    2. This spacing maintains the glyph’s true form across typefaces and platforms.
2. Data truncation with baseline ellipses
  1. Baseline ellipses [...] represent letters, words or phrases that aren’t shown. They also represent text truncation of a name or email address.
  2. Usage
    1. Type the ellipses as three periods in a row (or unicode character U2026) directly following the last letter shown.
