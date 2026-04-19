# Postman Test Scripts

This file summarizes the response checks used in the requests.

## Common Assertions

```javascript
pm.test("Status code is 200", function () {
  pm.response.to.have.status(200);
});
```

```javascript
pm.test("Response time should be below 500 ms", function () {
  pm.expect(pm.response.responseTime).to.be.below(500);
});
```

```javascript
pm.test("ID should be a string", function () {
  var jsonData = pm.response.json();
  pm.expect(jsonData.id).to.be.a("string");
});
```

## Update Request Timing Check (Task 8)

```javascript
pm.test("Response time should be below 400 ms", function () {
  pm.expect(pm.response.responseTime).to.be.below(400);
});
```

## Validation Outcome Summary

- Status checks passed with 200 OK in captured runs.
- Performance checks were applied (400-500 ms thresholds depending on task).
- Basic schema validation confirmed string id fields where needed.
