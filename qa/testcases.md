# Test Cases for JSONPlaceholder - Posts API

## TC-001: Get all posts
**Steps**  
1. Send GET request to `/posts`  
2. Check response  

**Expected**  
- Status code = 200  
- Response body contains 100 posts  

---

## TC-002: Get a single post
**Steps**  
1. Send GET request to `/posts/1`  
2. Check response  

**Expected**  
- Status code = 200  
- Response body contains post with `id = 1`  

---

## TC-003: Create a new post
**Steps**  
1. Send POST request to `/posts` with:
```json
{
  "title": "foo",
  "body": "bar",
  "userId": 1
}
"# JSONPlaceholder Manual Test Cases" 
