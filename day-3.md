### Day -3 


i have studied about the headers 

 think I should change my learning technique. I was thinking of first watching all the videos and making notes to build the foundation, which is great, but I think I should learn practically too. I learned about HTTP and what backend and frontend are, but just an overview of it, so I have decided to learn by coding too. I am going to code in Python as it is beginner-friendly and later learn Java. Learn the fundamentals and learn them practically too.


### Note 

## Representation Headers

### Content-Type
- Describes the media type of request or response e.g. JSON, HTML

### Content-Length
- Describes the size of the resource in bytes

### Content-Encoding
- Specifies by exactly the bytes follow

### ETag
- Unique identifier which is mainly used for caching

---

## Security Headers

### Strict-Transport-Security (HSTS)
- Ensures that the client only communicates with the server over HTTPS preventing potential downgrade attack

### Content-Security-Policy (CSP)
- Restricts the sources from which content like JavaScript, CSS and images can be loaded helping prevent cross-site scripting attacks

---

## Headers Overview

Headers is more information or metadata about the request/response.

**Example:** We can think headers as like the address on phone no written in the package

---

## Types of User Headers

### Request Headers
Sent by the client to server with the request itself

- **User-Agent** - Identifies whether it's Chrome, mobile, PC/laptop
- **Authorization** - Send token to identify the user
- **Cookie**
- **Accept** - What kind of content we are accepting like JSON file type

### General Headers (used in both)

- **Date**
- **Cache-Control** - It has info like max-age
- **Connection** - It has info to keep it alive or close it

---

## Additional Security Headers

### X-Frame-Options
- Prevents the web page from being embedded in iframe antiphishing clickjacking attack

### X-Content-Type-Options
- Ensures that the browser does not try to guess the MIME type of the content preventing MIME types sniffing attack

### Set-Cookie
- It is inaccessible with JavaScript and ensures that it is sent over HTTPS only
