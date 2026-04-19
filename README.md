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
- Evidence files are available under evidence/ (task-01-create-board.html to task-08-update-board.html).

## Repository Structure

- docs/: English technical notes and request/test references
- evidence/: Original exported task files and response screenshots from the exercise
- turkce/: Turkish summary documents

## Source Evidence

Raw task exports and image captures are preserved in evidence/:

- task-01-create-board.html to task-08-update-board.html
- evidence/resources/*

## How To Reproduce

1. Import the request flow into Postman (or create requests manually based on docs/request-reference.md).
2. Configure environment variables for credentials and dynamic IDs.
3. Run requests in sequence (Task 1 -> Task 8).
4. Review response body, status code, and execution time.

## Publish to GitHub

```bash
git init
git add .
git commit -m "Add Trello API testing project documentation"
git branch -M main
git remote add origin <YOUR_GITHUB_REPO_URL>
git push -u origin main
```
