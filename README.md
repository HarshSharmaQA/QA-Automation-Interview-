# QA Automation Interview Questions & Answers

If you want to improve in a **QA Automation role**, having a strong grasp of these commonly asked interview questions is essential.  
Dive in and prepare for your upcoming interview.

---

## **Selenium WebDriver**
1. **What are different types of locators in Selenium?**  
   - ID, Name, Class Name, Tag Name, Link Text, Partial Link Text, CSS Selector, XPath.  

2. **When do you use XPath over CSS locators?**  
   - When dealing with dynamic elements, complex hierarchy, or navigating between elements.  

3. **How to get a specific value from a dropdown and reuse it in verifications?**  
   - Use `Select` class in Selenium: `new Select(element).getFirstSelectedOption().getText()`.  

4. **When do we use JavaScript Executors?**  
   - When dealing with elements that are not interactable by Selenium's default methods.  

5. **Is it possible to validate Captcha using Selenium? If yes, how?**  
   - No, but can use third-party APIs like OCR or request developers for a test mode.  

6. **What should be the ideal way to store data using Selenium WebDriver only?**  
   - Use `Properties` file, JSON, Excel, or HashMap for storing test data.  

7. **Is it possible to use XPath like `parent/child/node/..`? If yes, provide an example where to use it?**  
   - Yes, `//div[@id='parent']/child::span` to navigate to specific elements.  

8. **What happens if you receive browser notifications during test automation execution?**  
   - Use ChromeOptions/FirefoxOptions to disable or auto-accept notifications.  

9. **Why does Stale Element Exception occur, and how to handle it?**  
   - When the element is no longer present in DOM; handle using explicit waits.  

10. **What is an Invalid Certificate Exception?**  
   - Happens due to SSL certificate issues; can be bypassed using ChromeOptions.  

---

## **APIs**
1. **What are the components of an HTTP request?**  
   - Method, URL, Headers, Body, and Query Parameters.  

2. **What is the difference between API and unit testing?**  
   - API testing validates request/response, unit testing checks individual code units.  

3. **What is an HTTP response?**  
   - A server's reply to a request containing status code, headers, and body.  

4. **How can we add validation points in Postman?**  
   - Use test scripts in the `Tests` tab with JavaScript assertions.  

5. **What do you understand by server-side validation?**  
   - Verification performed by the backend to ensure data integrity and security.  

6. **What is 3-tier architecture?**  
   - It consists of Presentation (UI), Business Logic, and Database layers.  

7. **What is the difference between web services and APIs?**  
   - Web services are a subset of APIs that use network-based communication.  

8. **What is REST, SOAP, and GraphQL in APIs?**  
   - REST (lightweight, stateless), SOAP (protocol-based), GraphQL (flexible queries).  

9. **What do you test in standalone APIs?**  
   - Functionality, performance, security, and response validation.  

10. **What do you test in 3rd-party integrated APIs?**  
   - Authentication, response consistency, rate limits, and error handling.  

---

## **Postman**
1. **When to use collections, environments, and global variables?**  
   - Collections group requests; environments store variables per setup; globals apply everywhere.  

2. **How to execute a collection end-to-end?**  
   - Use Postman Collection Runner or Newman CLI.  

3. **How to validate that an API response has the correct status code?**  
   - Use `pm.test("Status Code", function () { pm.response.to.have.status(200); });`  

4. **What happens when an API response returns Form Data instead of JSON, and how to validate it?**  
   - Parse form data manually in Postman or use `pm.response.text()` for validation.  

5. **How to set up Basic Auth in Postman?**  
   - Use Authorization tab and select "Basic Auth" with username & password.  

6. **Where do you store environment credentials?**  
   - Store in Postman Environment variables but avoid storing sensitive data in plain text.  

7. **How to save a demo response for an API request?**  
   - Click "Save Response" in Postman or log it using scripts.  

8. **How will you validate an API request if VPN is required for it to work?**  
   - Connect to VPN before making requests or use a proxy.  

9. **How do you filter results in an API request using Postman?**  
   - Use query parameters like `?status=active` or add JavaScript assertions.  

10. **How to set up custom headers in Postman?**  
   - Add key-value pairs in the Headers section.  

---

## **Git**
1. **What are the different stages in committing the code to GitHub?**  
   - Working Directory → Staging (`git add`) → Commit (`git commit -m`) → Push (`git push`).  

2. **Is it possible to revert changes in a remote repository? If yes, how?**  
   - Yes, using `git revert` or `git reset --hard` followed by `git push --force`.  

3. **When do you commit your code? After committing, how do you validate that everyone has the updated code?**  
   - Commit after verifying locally; validate using `git pull` and reviewing changes.  

4. **How to merge stashed changes in a local repository?**  
   - Use `git stash pop` or `git stash apply`.  

5. **Why do we need a `.gitignore` file? How do you add files to it?**  
   - To exclude files from tracking; add filenames or patterns inside `.gitignore`.  

---

## **TestNG**
1. **What is the execution format of tests in TestNG?**  
   - Defined using `@Test` annotation and controlled via `testng.xml`.  

2. **Can priority be negative for methods? If yes, what is the execution flow as per priority?**  
   - Yes, TestNG executes in ascending order (negative values run first).  

3. **What is the difference between `dependsOnMethods` and `dependsOnGroups`?**  
   - `dependsOnMethods` links tests at method level; `dependsOnGroups` links groups of tests.  

4. **What are the different ways to exclude tests in TestNG?**  
   - Using `exclude` in `testng.xml`, `@Test(enabled=false)`, or groups exclusion.  

5. **What does `threadPoolSize` mean in TestNG, and how does it work?**  
   - It sets parallel execution threads for a test method.  

6. **What are `@BeforeSuite` and `@AfterSuite` annotations?**  
   - `@BeforeSuite` runs setup before all tests; `@AfterSuite` runs cleanup after all tests.  

---

### **Pro Tip:**  
Familiarize yourself with these questions and practice answering them confidently.  
Let me know your thoughts and share this list with someone preparing for QA Automation roles. 🚀
