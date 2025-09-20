# JSONPlaceholder QA Tests

QA project for testing the [JSONPlaceholder](https://jsonplaceholder.typicode.com/) Posts API.  
Includes **manual test cases** and **automated Postman tests**.

---

## Project Structure

jsonplaceholder-qa-tests/
│── qa/
│ └── testcases.md # Manual test cases
│── postman/
│ └── JSONPlaceholder_Tests.postman_collection.json # Postman collection
│── README.md



---

## Manual Tests

Test cases cover:

- **GET /posts** → Expect 200, 100 posts  
- **GET /posts/1** → Expect 200, post with id = 1  
- **POST /posts** → Expect 201, new post with provided data  

---

## Automated Tests (Postman)

- Import collection: `postman/JSONPlaceholder_Tests.postman_collection.json`  
- Includes tests for GET and POST endpoints  
- Sample assertion:  

```javascript
pm.test("Status code is 200", () => pm.response.to.have.status(200));
# jsonplaceholder-qa-tests

## How to Run

Manual: Follow steps in qa/testcases.md

Automated: Import Postman collection → Click Run → Check results


Skills Demonstrated

API Manual Testing

Postman Automated Testing

QA Documentation & Repo Structuring


