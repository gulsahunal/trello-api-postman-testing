# Trello API Testing with Postman

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
- This repository is presented as a live showcase.

## Live Showcase (GitHub Pages)

- Language selector: [Open Showcase](https://gulsahunal.github.io/trello-api-postman-testing/evidence/index.html)
- Turkish index: [Open Turkish Task List](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/index.html)
- English index: [Open English Task List](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/index.html)

### Turkish Task Pages

- Task 01: [Create Board (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-01-create-board.html)
- Task 02: [Create Left List (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-02-create-left-list.html)
- Task 03: [Create Right List (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-03-create-right-list.html)
- Task 04: [Create Left Card (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-04-create-left-card.html)
- Task 05: [Create Right Card (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-05-create-right-card.html)
- Task 06: [Delete Card (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-06-delete-card.html)
- Task 07: [Get Board Data (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-07-get-board-data.html)
- Task 08: [Update Board (TR)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/tr/task-08-update-board.html)

### English Task Pages

- Task 01: [Create Board (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-01-create-board.html)
- Task 02: [Create Left List (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-02-create-left-list.html)
- Task 03: [Create Right List (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-03-create-right-list.html)
- Task 04: [Create Left Card (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-04-create-left-card.html)
- Task 05: [Create Right Card (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-05-create-right-card.html)
- Task 06: [Delete Card (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-06-delete-card.html)
- Task 07: [Get Board Data (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-07-get-board-data.html)
- Task 08: [Update Board (EN)](https://gulsahunal.github.io/trello-api-postman-testing/evidence/en/task-08-update-board.html)

## Repository Structure

- docs/: English technical notes and request/test references
- evidence/: Live showcase pages for Turkish and English evidence views
- turkce/: Turkish summary documents
