# Task Tracker — Patch Notes

## Summary of Changes Made
- Fixed the search and status filter SQL logic so the correct tasks appear.
- Fixed the pagination issue by resetting to page 1 when the search term or status filter changes.
- Improved API request handling to manage loading, errors, and outdated search results.
- Updated the Oracle SQL reference to match the corrected search logic and task ordering.

## What I Chose Not to Change
- Kept archived tasks hidden because the expected behavior is not clearly specified.
- Left the existing pagination implementation unchanged.

## Biggest Remaining Risk
- The backend loads all matching tasks before displaying one page, which could become slow if the number of tasks grows.

## Tools Used
- Used ChatGPT to help debug the code and understand possible fixes. Tested the changes locally.