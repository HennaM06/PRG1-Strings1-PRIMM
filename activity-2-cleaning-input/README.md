# Activity 2: Cleaning what people typed

File: `clean_signups.py`

Five people signed up. Some of them are the same person. The program works out
how many are actually distinct.

## Predict

- How many entries are accepted?
3 
- Which ones are rejected, and why?
2 - Because they have capitalised letters 
- What does the final line say?
3 Unique sign ups from 5 entries 
## Run

Execute and compare.

## Investigate

- Look at the five raw entries. To a human, how many different people are there?
  The program agrees. What did it have to do first to get there?
- `clean` does two things in one line. Name both, and say what each one removes.
- Delete `.strip()` from `clean` and predict the new output before running it.
  Then delete `.lower()` instead. Which one mattered more, and why?

.strip() removed spaces at beginning and end of text
.lower()converts all letters to lowercase 

- The check is `if cleaned in accepted:`. What would happen if it compared the
  raw `entry` instead?

  The code would not spot duplicates and entries with different spaces or capital letters would be accepted as new sign ups 

## Modify

- Someone signs up as `ALICE@EXAMPLE.COM`. Confirm the program already handles
  it, and say which line does the work.

  The programme handles it in the return entry.strip().lower() line


- A trailing full stop gets typed by accident: `alice@example.com.`. The program
  treats that as a new person. Should it? Decide with your partner before you
  change anything.

  The current system will treat it as a different sign up - but it shouldn't as most programmes will acknowledge that it is a spelling error

> Normalising input before comparing it is one of the most common jobs in real
> software, and forgetting to do it is one of the most common faults. You will
> need this again in about an hour.
