#challenge-5

Task description: Blind SQL injection. Anayze php file and python file. Extract password. 

Analyzis:
1. Analyze php file.
~$db = new mysqli('127.0.0.1', 'teni', 'teni', 'sqli_challenge');

---this line creates a connection to MySQL database.
---host:127.0.0.1
---username:'teni'
---password:'teni'
---database name:'sqli_challenge'

~echo is a php command to send all that is written in its quotes to the browser.(page is generated dynamically ie, generated in real-time)

---doc type: html (if not mentioned then browser may switch to quirks mode)
---html language: english
---Note: In php, double quotes-smart(variables are evaluated), single quotes-literal(variables not evaluated ie, takes what's written in the quote exactly.)
---UTF-8 to interpret the html page.
---filters to avoid during sql inference: _.()"or" "and" substrings
---bypass the login as the admin by getting its password.

~if (isset($_GET['pw'])) {
---checks if the URL contains a parameter named "pw"

~if ,_() found, browser shows "NO HACK ~_~"
~if and,or,substring found, browser shows "HEHE"

~$query = "select * from users where id='guest' and pw='{$_GET['pw']}'";
---
