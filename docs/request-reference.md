# Request Reference

This file summarizes the request definitions used in the Postman-based Trello API exercise.

## Environment Variables Used

- apikey
- token
- idboard
- idlist
- idcard
- id (board id in update task)
- type

Note: This reference normalizes the API key variable to `apikey`.

## Request List

### Task 1 - Create a Board
- Method: POST
- URL: https://api.trello.com/1/boards/?name={name}&key={{apikey}}&token={{token}}
- Purpose: Create a new board.

### Task 2 - Create Left List
- Method: POST
- URL: https://api.trello.com/1/lists?name={left}&idBoard={{idboard}}&key={{apikey}}&token={{token}}&pos=top
- Purpose: Create the left/top list.

### Task 3 - Create Right List
- Method: POST
- URL: https://api.trello.com/1/lists?name={right}&idBoard={{idboard}}&key={{apikey}}&token={{token}}&pos=bottom
- Purpose: Create the right/bottom list.

### Task 4 - Create Card in Left List
- Method: POST
- URL: https://api.trello.com/1/cards?idList={{idlist}}&key={{apikey}}&token={{token}}
- Purpose: Add a card in the left list.

### Task 5 - Create Card in Right List
- Method: POST
- URL: https://api.trello.com/1/cards?idList={{idlist}}&key={{apikey}}&token={{token}}
- Purpose: Add a card in the right list.

### Task 6 - Delete a Card
- Method: DELETE
- URL: https://api.trello.com/1/cards/{{idcard}}?key={{apikey}}&token={{token}}&idcard={{idcard}}
- Purpose: Delete a card created in previous tasks.

### Task 7 - Get Board Data
- Method: GET
- URL: https://api.trello.com/1/members/me/boards?key={{apikey}}&token={{token}}
- Purpose: Retrieve the authenticated user's boards.

### Task 8 - Update a Board
- Method: PUT
- URL: https://api.trello.com/1/boards/{{id}}/?type={{type}}&key={{apikey}}&token={{token}}
- Purpose: Update board information (for example, name or description).
