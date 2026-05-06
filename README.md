# Week 9 Homework: The Case of the Missing Festival Lanterns

## Student Info

Name: Aqush Limbu  
Student number: TODO  
GitHub username: TODO  

---

## Summary

This program analyzes festival lantern records to identify problems such as missing lanterns, unexpected lanterns, duplicates, and incorrect placements. The function `analyze_lanterns` takes a set of expected lanterns, a log of lantern entries with their sections, and a dictionary of correct sections. It processes the log to track which lanterns were seen, counts how many times each section appears, and checks whether each expected lantern is in the correct section. Finally, it returns a report dictionary containing all the results.

---

## Approach

- First, I created sets and dictionaries to store seen lanterns, duplicate lanterns, section counts, and wrong section data.
- Then, I looped through each record in `lantern_log`.
- I added each lantern to a set to track seen lanterns.
- I used another set to detect duplicates efficiently.
- I updated a dictionary to count how many lanterns appear in each section.
- I checked if each expected lantern was in the correct section and recorded the first wrong occurrence.
- After the loop, I used set operations to find missing and unexpected lanterns.
- Finally, I returned all results in a dictionary.

---

## How I Used Dictionaries and Sets

```text
Sets were used to:
- Track all seen lanterns
- Identify duplicate lanterns
- Find missing lanterns
- Find unexpected lanterns

Dictionaries were used to:
- Count lanterns in each section (count_by_section)
- Store wrong section details (wrong_section_lanterns)

Sets are useful because they provide fast lookups and prevent duplicates.
Dictionaries are useful for mapping and counting values efficiently.