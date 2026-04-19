# Request Reference

This file summarizes the request definitions used in the Postman-based Trello API exercise.

## Environment Variables Used

- apikey or Apikey
- token
- id (board id in update/get tasks)
- idboard
- idlist
- idcard
- type

Note: The original exported tasks use both apikey and Apikey. For consistency in a real project, use a single variable naming style.

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
- URL: https://api.trello.com/1/cards/{{idcard}}?key={{Apikey}}&token={{token}}&idcard={{idcard}}
- Purpose: Delete a card created in previous tasks.

### Task 7 - Get Cards on a Board (as implemented in source)
- Method: GET
- URL: https://api.trello.com/1/members/me/boards?key={{Apikey}}&token={{token}}&id={{id}}
- Purpose: Retrieve board-related data for the authenticated user.

### Task 8 - Update a Board
- Method: PUT
- URL: https://api.trello.com/1/boards/{{id}}/?type={{type}}&key={{Apikey}}&token={{token}}
- Purpose: Update board information (for example, name or description).
