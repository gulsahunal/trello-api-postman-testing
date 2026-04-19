# Trello API Testing with Postman

[Türkçe](turkce/README.md)

This project documents a practical Trello API testing workflow executed in Postman.
Requests were made to create, list, update, and delete Trello resources, using API key and token authentication for secure access.
Response data and timing were validated to improve API integration and testing skills.

## What Was Tested

| Task | Action | Method | Endpoint |
| --- | --- | --- | --- |
| 1 | Create a board | POST | /1/boards |
| 2 | Create left list (top) | POST | /1/lists |
| 3 | Create right list (bottom) | POST | /1/lists |
| 4 | Create card in left list | POST | /1/cards |
| 5 | Create card in right list | POST | /1/cards |
| 6 | Delete a card | DELETE | /1/cards/{idcard} |
| 7 | Get board-related data | GET | /1/members/me/boards |
| 8 | Update board details | PUT | /1/boards/{id} |

## Authentication and Security

- Trello API key and token are passed as query parameters in Postman requests.
- Sensitive values should be stored in Postman environment variables.
- Do not commit real secrets to GitHub.

## Validation Strategy

Postman tests were used to validate:

- HTTP status code (200)
- Response time thresholds (mostly < 500 ms, update request < 400 ms)
- Response schema basics (for example, id is a string)

## Test Result Summary

- 8/8 tasks completed successfully in the documented run.
- Expected HTTP status responses were received for each request.
- Response time assertions passed under defined thresholds.
- This repository is published as a project presentation.

## Task Pages

- Open all tasks: [Task List](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/index.html)

## Repository Structure

- docs/: English technical notes and request/test references
- evidence/: Turkish and English task pages for project presentation
- turkce/: Turkish summary documents
