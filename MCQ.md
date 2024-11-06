JavaScript Code Snippets - TCS IPA Important MCQs

1. What is the output of: console.log(1 + "2" + "2")
   Answer: "122" (Type coercion converts 1 to string and concatenates)

2. What is the output of: console.log(1 + +"2" + "2")
   Answer: "32" (Unary plus converts "2" to number, then addition happens left to right)

3. console.log(typeof typeof 1)
   Answer: "string" (typeof 1 returns "number" which is a string)

4. console.log(false == '0')
   Answer: true (Type coercion converts both to numbers)

5. console.log(null === undefined)
   Answer: false (Strict equality checks type, which are different)

6. console.log(typeof NaN)
   Answer: "number" (NaN is a special number value)

7. console.log("hello" - 1)
   Answer: NaN (Cannot subtract number from string)

8. console.log([] + {})
   Answer: "[object Object]" (Arrays convert to empty string, object converts to string representation)

9. console.log(true + false)
   Answer: 1 (true=1, false=0 in numeric context)

10. console.log([1,2,3] + [4,5,6])
    Answer: "1,2,34,5,6" (Arrays convert to strings and concatenate)

11. console.log(0.1 + 0.2 === 0.3)
    Answer: false (Floating point precision issue)

12. console.log('b' + 'a' + +'a' + 'a')
    Answer: "baNaNa" (+'a' becomes NaN)

13. console.log(!!"")
    Answer: false (Empty string is falsy)

14. console.log([] == ![])
    Answer: true (Complex type coercion)

15. console.log({} + [])
    Answer: 0 (Interpreted as +[] which is 0)

16. console.log(typeof (() => {}))
    Answer: "function" (Arrow function typeof)

17. console.log(2 in [1,2,3])
    Answer: true ('in' checks index existence)

18. console.log(typeof [])
    Answer: "object" (Arrays are objects)

19. console.log(parseFloat('12.3.4'))
    Answer: 12.3 (Parses until invalid decimal)

20. console.log(Math.max())
    Answer: -Infinity (No arguments case)

21. console.log(typeof null)
    Answer: "object" (Historical JavaScript quirk)

22. console.log('2' > '12')
    Answer: true (String comparison is lexicographical)

23. console.log(3 > 2 > 1)
    Answer: false (Evaluates left to right: (3>2)>1 -> true>1 -> 1>1 -> false)

24. console.log(typeof (1n))
    Answer: "bigint" (BigInt literal type)

25. console.log(+"")
    Answer: 0 (Empty string converts to 0)

26. console.log([]+[])
    Answer: "" (Empty arrays convert to empty strings)

27. console.log(1/0)
    Answer: Infinity (Division by zero)

28. console.log(0.1 * 0.2)
    Answer: 0.020000000000000004 (Floating point precision)

29. console.log(999999999999999)
    Answer: 999999999999999 (Max precise integer)

30. console.log([1,2] == "1,2")
    Answer: true (Array converts to string for comparison)

31. What is the output of: System.out.println("5" + 2 + 3)
    Answer: "523" (String concatenation happens left to right)

32. What is the output of: System.out.println(2 + 3 + "5")
    Answer: "55" (Addition happens first, then string concatenation)

33. System.out.println(10 + 20 + "Java" + 10 + 20)
    Answer: "30Java1020" (Left to right evaluation)

34. System.out.println(String.valueOf(true) == "true")
    Answer: false (String objects comparison, not value)

35. System.out.println(10.0/0)
    Answer: Infinity (Floating point division by zero)

36. System.out.println(10/0.0)
    Answer: Infinity (Floating point division by zero)

37. System.out.println(0.0/0)
    Answer: NaN (Not a Number result)

38. System.out.println(23%2.5)
    Answer: 0.5 (Modulus with decimal)

39. char[] ch = {'j', 'a', 'v', 'a'}; String s = new String(ch);
    Answer: "java" (Character array to String conversion)

40. System.out.println('A' + 'B')
    Answer: 131 (ASCII values are added)

41. System.out.println('A' + "B")
    Answer: "AB" (String concatenation)

42. System.out.println(10 >> 1)
    Answer: 5 (Right shift divides by 2)

43. System.out.println(-10 >> 1)
    Answer: -5 (Sign preserved in arithmetic right shift)

44. System.out.println(Integer.MIN_VALUE-1)
    Answer: Integer.MAX_VALUE (Integer overflow)

45. System.out.println(Math.min(Double.MIN_VALUE, 0.0d))
    Answer: 0.0 (Double.MIN_VALUE is positive)

46. System.out.println(1.0/0 == Double.POSITIVE_INFINITY)
    Answer: true (Infinity comparison)

47. System.out.println(Math.min(float.NaN, 0.0f))
    Answer: NaN (NaN comparison always returns NaN)

48. System.out.println("hello".charAt(0) == 'h')
    Answer: true (Character comparison)

49. System.out.println(010)
    Answer: 8 (Octal number representation)

50. System.out.println(0x10)
    Answer: 16 (Hexadecimal number representation)

51. System.out.println(null + "test")
    Answer: "nulltest" (null converts to "null" string)

52. System.out.println((int)(char)(byte)-1)
    Answer: 65535 (Type conversion chain)

53. System.out.println(2147483647+1)
    Answer: -2147483648 (Integer overflow)

54. System.out.println(1/0.0 == 2/0.0)
    Answer: true (Both are positive infinity)

55. System.out.println("string".substring(3,3))
    Answer: "" (Empty string - same start and end index)

56. System.out.println(Long.toHexString(0x100000000L + 0xcafebabe))
    Answer: "1cafebabe" (Long arithmetic and hex conversion)

57. System.out.println(Integer.parseInt("10",2))
    Answer: 2 (Binary string to decimal)

58. System.out.println("Java".indexOf('a',2))
    Answer: 3 (Index of 'a' starting from position 2)

59. System.out.println(Math.round(2.5f))
    Answer: 3 (Rounds to nearest integer)

60. System.out.println("ABC".compareTo("ABC"))
    Answer: 0 (Equal strings comparison)

# Java Normal


1. Which access modifier makes class members accessible only within the same package?
   - default (package-private)

2. What is the output of System.out.println(1 + 2 + "3")?
   - 33

3. Which collection doesn't allow duplicate elements?
   - Set

4. What is the default value of instance variables of type int?
   - 0

5. Which keyword is used to prevent method overriding?
   - final

6. What is the superclass of all Java classes?
   - Object

7. Which interface is used to create threads in Java?
   - Runnable

8. What happens when a constructor throws an exception?
   - Object creation fails

9. Which collection type maintains insertion order?
   - LinkedHashSet

10. What is the return type of constructor?
    - No return type

11. Which operator is used for object type comparison?
    - instanceof

12. What is the default size of ArrayList?
    - 10

13. Which method must be implemented in thread creation?
    - run()

14. What is the scope of protected members?
    - Package and subclasses

15. Which collection allows null elements?
    - ArrayList

16. What happens when main() is declared as private?
    - Compilation error

17. Which keyword is used for exception handling?
    - try

18. What is the default value of boolean?
    - false

19. Which interface is used for sorting objects?
    - Comparable

20. What is the output of 5/2 in Java?
    - 2

21. Which collection type is synchronized by default?
    - Vector

22. What is the purpose of static blocks?
    - Class initialization

23. Which method is called when object is garbage collected?
    - finalize()

24. What is the superclass of String?
    - Object

25. Which keyword creates constant variables?
    - final

26. What is the default access modifier?
    - package-private

27. Which interface is used for implementation of hashCode()?
    - Hashable

28. What is the size of int in Java?
    - 4 bytes

29. Which collection doesn't allow null elements?
    - Hashtable

30. What is autoboxing in Java?
    - Primitive to wrapper conversion

31. Which method must be overridden with equals()?
    - hashCode()

32. What is the default capacity of HashMap?
    - 16

33. Which keyword is used for method overriding?
    - @Override

34. What is the purpose of volatile keyword?
    - Thread synchronization

35. Which collection maintains natural ordering?
    - TreeSet

36. What is the return type of equals()?
    - boolean

37. Which operator has highest precedence?
    - ()

38. What is the purpose of super keyword?
    - Access parent members

39. Which interface is used for implementing comparator?
    - Comparator

40. What is the default value of Object reference?
    - null

41. Which collection type allows duplicate elements?
    - List

42. What is the purpose of static methods?
    - Class level operations

43. Which keyword is used for interface implementation?
    - implements

44. What is the purpose of break statement?
    - Loop termination

45. Which collection is better for frequent insertions?
    - LinkedList

46. What is the scope of private members?
    - Class only

47. Which operator is used for string concatenation?
    - +

48. What is the purpose of abstract classes?
    - Partial implementation

49. Which method is used to get array length?
    - length

50. What is the default value of char?
    - '\u0000'

51. Which collection type is thread-safe?
    - ConcurrentHashMap

52. What is the purpose of this keyword?
    - Current object reference

53. Which keyword is used for inheritance?
    - extends

54. What is the purpose of finally block?
    - Cleanup operations

55. Which collection is better for frequent retrievals?
    - ArrayList

56. What is the purpose of static variables?
    - Class level storage

57. Which operator is used for bitwise AND?
    - &

58. What is the purpose of interface?
    - Multiple inheritance

59. Which method is called when object is created?
    - constructor

60. What is the purpose of package in Java?
    - Namespace management


61. What is the primary key constraint used for?
    - Unique record identification

62. Which SQL clause is used for filtering rows?
    - WHERE

63. What is the default port for PostgreSQL?
    - 5432

64. Which command is used to modify table structure?
    - ALTER

65. What does ACID stand for in databases?
    - Atomicity, Consistency, Isolation, Durability

66. Which JOIN returns all matches and non-matches?
    - FULL OUTER JOIN

67. What is the purpose of GROUP BY?
    - Aggregate data grouping

68. Which function returns current date in PostgreSQL?
    - CURRENT_DATE

69. What is the maximum size of VARCHAR in PostgreSQL?
    - 10485760 bytes

70. Which constraint ensures data integrity?
    - FOREIGN KEY

71. What is the purpose of HAVING clause?
    - Filter grouped data

72. Which command removes table data?
    - TRUNCATE

73. What is the purpose of INDEX?
    - Faster data retrieval

74. Which function counts non-null values?
    - COUNT

75. What is a view in SQL?
    - Virtual table

76. Which operator tests for NULL values?
    - IS NULL

77. What is the purpose of DISTINCT?
    - Remove duplicates

78. Which command modifies table data?
    - UPDATE

79. What is a stored procedure?
    - Saved SQL code

80. Which clause sorts query results?
    - ORDER BY

81. What is the purpose of COMMIT?
    - Save transactions

82. Which operator combines result sets?
    - UNION

83. What is the purpose of ROLLBACK?
    - Undo transactions

84. Which function returns current time?
    - CURRENT_TIME

85. What is a trigger in PostgreSQL?
    - Automatic procedure

86. Which clause limits result rows?
    - LIMIT

87. What is the purpose of CASCADE?
    - Automatic updates/deletes

88. Which function rounds numbers?
    - ROUND

89. What is a sequence in PostgreSQL?
    - Auto-increment object

90. Which command removes a table?
    - DROP TABLE

91. What is the purpose of COALESCE?
    - Handle NULL values

92. Which operator matches patterns?
    - LIKE

93. What is a cursor?
    - Result set pointer

94. Which function concatenates strings?
    - CONCAT

95. What is the purpose of VACUUM?
    - Database maintenance

96. Which constraint prevents NULL?
    - NOT NULL

97. What is the purpose of SERIAL?
    - Auto-increment columns

98. Which function gets substring?
    - SUBSTRING

99. What is a materialized view?
    - Stored query results

100. Which command grants permissions?
    - GRANT

101. What is the purpose of EXISTS?
    - Subquery testing

102. Which function counts all rows?
    - COUNT(*)

103. What is database normalization?
    - Data organization

104. Which operator checks multiple values?
    - IN

105. What is the purpose of WITH clause?
    - Common table expressions

106. Which function gets current user?
    - CURRENT_USER

107. What is a schema in PostgreSQL?
    - Namespace for objects

108. Which command revokes permissions?
    - REVOKE

109. What is the purpose of EXPLAIN?
    - Query analysis

110. Which operator checks ranges?
    - BETWEEN

111. What is transaction isolation?
    - Concurrent access control

112. Which function converts data types?
    - CAST

113. What is the purpose of CLUSTER?
    - Physical row ordering

114. Which command copies data?
    - INSERT INTO

115. What is a composite key?
    - Multiple column key


116. What command displays current directory path?
    - pwd

117. Which command lists directory contents?
    - ls

118. What does chmod 777 indicate?
    - Full permissions for all

119. Which command creates directories?
    - mkdir

120. What is the purpose of grep command?
    - Pattern searching

121. Which command removes files?
    - rm

122. What is the root user ID?
    - 0

123. Which command displays system processes?
    - ps

124. What does the pipe operator (|) do?
    - Command chaining

125. Which command changes directories?
    - cd

126. What command shows disk usage?
    - df

127. Which signal terminates processes?
    - SIGKILL (9)

128. What command displays file contents?
    - cat

129. Which command finds files?
    - find

130. What is the purpose of chmod?
    - Change permissions

131. Which command copies files?
    - cp

132. What does ls -l show?
    - Detailed listing

133. Which command moves files?
    - mv

134. What is /etc directory for?
    - System configuration

135. Which command shows system uptime?
    - uptime

136. What command modifies file timestamps?
    - touch

137. Which command shows memory usage?
    - free

138. What does cd .. do?
    - Move up directory

139. Which command shows command history?
    - history

140. What is /home directory for?
    - User directories

141. Which command compresses files?
    - gzip

142. What does ls -a show?
    - All files including hidden

143. Which command shows network interfaces?
    - ifconfig

144. What is /bin directory for?
    - Essential commands

145. Which command shows file type?
    - file

146. What does chmod +x do?
    - Add execute permission

147. Which command counts words?
    - wc

148. What is /tmp directory for?
    - Temporary files

149. Which command shows current user?
    - whoami

150. What does echo $PATH show?
    - Command search path

151. Which command shows disk partition info?
    - fdisk

152. What is shell in Unix?
    - Command interpreter

153. Which command shows calendar?
    - cal

154. What does sudo command do?
    - Superuser access

155. Which command sorts file content?
    - sort

156. What is cron used for?
    - Scheduled tasks

157. Which command shows manual pages?
    - man

158. What does tar command do?
    - Archive files

159. Which command shows logged users?
    - who

160. What is shell scripting?
    - Automated commands

161. Which command shows CPU info?
    - lscpu

162. What does ping command do?
    - Network testing

163. Which command sets file ownership?
    - chown

164. What is /dev directory for?
    - Device files

165. Which command shows directory tree?
    - tree


166. What is the correct HTML element for inserting a line break?
    - <br>

167. Which CSS property controls text size?
    - font-size

168. How do you write "Hello World" in an alert box using JavaScript?
    - alert("Hello World");

169. What is the correct HTML for creating a hyperlink?
    - <a href="url">link text</a>

170. Which CSS property is used to change background color?
    - background-color

171. How do you declare a JavaScript variable?
    - var x;

172. What is the correct HTML for making a checkbox?
    - <input type="checkbox">

173. How do you make a list that lists its items with squares?
    - list-style-type: square;

174. How do you find the length of a string in JavaScript?
    - string.length

175. Which HTML attribute specifies an alternate text for an image?
    - alt

176. Which CSS property controls the text color?
    - color

177. What is the correct way to write a JavaScript array?
    - var colors = ["red", "green", "blue"]

178. What does CSS stand for?
    - Cascading Style Sheets

179. How do you round the number 7.25 to the nearest integer in JavaScript?
    - Math.round(7.25)

180. Which HTML element defines navigation links?
    - <nav>

181. How do you add a comment in CSS?
    - /* comment */

182. How do you find the number with the highest value of x and y?
    - Math.max(x,y)

183. What is the correct HTML element for the largest heading?
    - <h1>

184. Which CSS property sets the space between lines?
    - line-height

185. How do you create a function in JavaScript?
    - function myFunction()

186. What is the correct HTML for making a text input field?
    - <input type="text">

187. How do you make each word in a text start with a capital letter?
    - text-transform: capitalize;

188. How do you write an IF statement in JavaScript?
    - if (condition) {}

189. Which HTML element is used to specify a header for a document?
    - <header>

190. How do you select elements with class name "test"?
    - .test

191. What is the correct way to write a JavaScript object?
    - var person = {name:"John", age:30}

192. Which HTML element defines the title of a document?
    - <title>

193. Which CSS property controls text alignment?
    - text-align

194. How do you call a function named "myFunction"?
    - myFunction()

195. How do you insert a comment in HTML?
    - <!-- comment -->

196. How do you make a text bold in CSS?
    - font-weight: bold;

197. How do you create an array in JavaScript?
    - var array = []

198. Which HTML attribute is used to define inline styles?
    - style

199. How do you make a text italic in CSS?
    - font-style: italic;

200. What is the correct JavaScript syntax to change content of HTML element?
    - document.getElementById("demo").innerHTML = "Hello"

201. What is the correct HTML for inserting an image?
    - <img src="image.jpg">

202. Which CSS property is used to change the font of an element?
    - font-family

203. How do you declare a JavaScript constant?
    - const x = 5;

204. Which HTML element defines a table?
    - <table>

205. How do you add shadows to elements in CSS?
    - box-shadow

206. How do you write a FOR loop in JavaScript?
    - for(let i=0; i<5; i++)

207. What is the correct HTML for creating a form?
    - <form>

208. Which CSS property sets element width?
    - width

209. How do you convert string to integer in JavaScript?
    - parseInt()

210. Which HTML element is used to define important text?
    - <strong>

211. How do you set border style in CSS?
    - border-style

212. What will Math.floor(4.7) return in JavaScript?
    - 4

213. Which HTML element defines footer section?
    - <footer>

214. How do you set text to center in CSS?
    - text-align: center;

215. How do you find elements by class name in JavaScript?
    - getElementsByClassName()

216. What is the correct HTML for adding background color?
    - <body style="background-color:yellow;">

217. Which CSS property adds rounded corners?
    - border-radius

218. How do you check if variable is undefined?
    - typeof x === "undefined"

219. Which HTML tag is used for ordered list?
    - <ol>

220. How do you set element position to fixed in CSS?
    - position: fixed;

221. How do you check length of array in JavaScript?
    - array.length

222. What is semantic HTML?
    - Meaningful markup

223. How do you create responsive layout in CSS?
    - @media queries

224. What is event bubbling in JavaScript?
    - Event propagation upwards

225. Which HTML5 element defines article?
    - <article>

226. How do you add text shadow in CSS?
    - text-shadow

227. How do you add element to array in JavaScript?
    - push()

228. What defines viewport in HTML5?
    - <meta name="viewport">

229. How do you make element float right?
    - float: right;

230. What is callback function in JavaScript?
    - Function passed as argument

231. What is localStorage in JavaScript?
    - Web storage API

232. How do you specify character encoding in HTML?
    - <meta charset="UTF-8">

233. What is flexbox in CSS?
    - Flexible layout model

234. How do you check if element exists in JavaScript?
    - document.getElementById() !== null

235. What is purpose of data- attributes?
    - Custom data storage

236. How do you create grid layout in CSS?
    - display: grid;

237. What is promise in JavaScript?
    - Asynchronous operation

238. What is role attribute in HTML?
    - Accessibility information

239. How do you create animation in CSS?
    - @keyframes

240. What is closure in JavaScript?
    - Inner function access

241. What is srcset attribute?
    - Responsive images

242. How do you center div in CSS?
    - margin: auto;

243. What is prototype in JavaScript?
    - Object inheritance

244. What is purpose of main tag?
    - Main content wrapper

245. How do you implement CSS variables?
    - --variable-name



SQL MCQs for TCS IPA:

1. What is the default port for SQL Server?
   Answer: 1433 (Standard port assigned by IANA for SQL Server)

2. Which SQL function returns current date and time?
   Answer: GETDATE() (Built-in function for current timestamp)

3. What is the maximum size of varchar in SQL Server?
   Answer: 8000 characters (Storage limitation for non-unicode strings)

4. Which statement creates a new table?
   Answer: CREATE TABLE (DDL command to define new table structure)

5. What does ACID stand for?
   Answer: Atomicity, Consistency, Isolation, Durability (Database transaction properties)

6. Which JOIN shows all matching records from both tables?
   Answer: INNER JOIN (Returns only matched records)

7. What does GROUP BY do?
   Answer: Groups rows with similar values (For aggregate functions)

8. Which constraint ensures referential integrity?
   Answer: FOREIGN KEY (Links tables through relationships)

9. What is a view?
   Answer: Virtual table (Stored SELECT query)

10. Which command removes a table and its data?
    Answer: DROP TABLE (Permanently deletes table structure and data)

11. What does HAVING clause do?
    Answer: Filters grouped data (WHERE for GROUP BY)

12. Which operator checks NULL values?
    Answer: IS NULL (Cannot use = for NULL comparison)

13. What is the purpose of DISTINCT?
    Answer: Removes duplicates (Returns unique values only)

14. Which function counts rows?
    Answer: COUNT() (Aggregate function for counting)

15. What is a stored procedure?
    Answer: Precompiled SQL statements (Reusable code blocks)

16. Which clause sorts results?
    Answer: ORDER BY (Specifies sort order)

17. What does COMMIT do?
    Answer: Saves transactions (Makes changes permanent)

18. Which operator combines results?
    Answer: UNION (Merges result sets)

19. What is an index?
    Answer: Database structure for faster retrieval (Improves query performance)

20. Which constraint prevents NULL values?
    Answer: NOT NULL (Ensures column always has value)

21. What is normalization?
    Answer: Data organization process (Reduces redundancy)

22. Which operator checks multiple values?
    Answer: IN (Alternative to multiple OR conditions)

23. What is a trigger?
    Answer: Automatic procedure (Executes on table events)

24. Which function gets substring?
    Answer: SUBSTRING() (Extracts part of string)

25. What is a primary key?
    Answer: Unique identifier (Ensures record uniqueness)

26. Which clause limits results?
    Answer: TOP/LIMIT (Restricts number of rows)

27. What is an alias?
    Answer: Alternative name (Temporary name for column/table)

28. Which operator matches patterns?
    Answer: LIKE (String pattern matching)

29. What is a transaction?
    Answer: Unit of work (Group of SQL statements)

30. Which function rounds numbers?
    Answer: ROUND() (Mathematical rounding)

31. What is a cursor?
    Answer: Row pointer (Processes result set row by row)

32. Which operator checks ranges?
    Answer: BETWEEN (Range comparison)

33. What is collation?
    Answer: Character set rules (Defines string comparison)

34. Which function converts data types?
    Answer: CAST/CONVERT (Data type conversion)

35. What is deadlock?
    Answer: Resource conflict (Circular dependency between transactions)

PostgreSQL MCQs:

1. What is the default port for PostgreSQL?
   Answer: 5432 (Standard PostgreSQL listening port)

2. Which data type stores unlimited length string?
   Answer: TEXT (Variable unlimited length)

3. What is SERIAL data type?
   Answer: Auto-incrementing integer (Automatic sequence)

4. Which command shows current database?
   Answer: SELECT current_database() (System function)

5. What is a schema?
   Answer: Namespace for database objects (Logical container)

6. Which operator for pattern matching?
   Answer: ~* (Case-insensitive regex)

7. What is VACUUM?
   Answer: Maintenance operation (Reclaims storage)

8. Which function gets current user?
   Answer: current_user (Session user)

9. What is inheritance in tables?
   Answer: Table hierarchy (Parent-child relationship)

10. Which operator for JSON containment?
    Answer: @> (Contains operator)

11. What is EXPLAIN ANALYZE?
    Answer: Query execution plan (Performance analysis)

12. Which function aggregates arrays?
    Answer: array_agg() (Creates array from rows)

13. What is a materialized view?
    Answer: Stored query results (Cached view)

14. Which operator for full text search?
    Answer: @@ (Text search match)

15. What is NOTIFY?
    Answer: Asynchronous notification (Inter-process communication)

16. Which function generates UUID?
    Answer: gen_random_uuid() (Unique identifier)

17. What is LISTEN?
    Answer: Notification receiver (Catches NOTIFY)

18. Which operator for range types?
    Answer: && (Range overlap)

19. What is a foreign table?
    Answer: External data link (References external data)

20. Which function gets transaction ID?
    Answer: txid_current() (Current transaction)

21. What is pg_dump?
    Answer: Backup tool (Database export)

22. Which function for window frames?
    Answer: over() (Window function)

23. What is REINDEX?
    Answer: Index rebuild (Reconstructs index)

24. Which operator for array elements?
    Answer: ANY (Array comparison)

25. What is point-in-time recovery?
    Answer: WAL replay (Recovery to specific time)

26. Which function for JSON extraction?
    Answer: jsonb_extract_path() (Path navigation)

27. What is HOT update?
    Answer: Heap-Only Tuples (Optimized updates)

28. Which operator for geometric comparison?
    Answer: <-> (Distance operator)

29. What is tablespace?
    Answer: Storage location (Physical storage)

30. Which function for row locking?
    Answer: FOR UPDATE (Exclusive lock)

31. What is WAL?
    Answer: Write-Ahead Logging (Transaction logging)

32. Which operator for full join?
    Answer: FULL OUTER JOIN (All rows)

33. What is pgbench?
    Answer: Benchmarking tool (Performance testing)

34. Which function for array unnesting?
    Answer: unnest() (Array to rows)

35. What is autovacuum?
    Answer: Automatic maintenance (Background cleanup)



HTML MCQs for TCS IPA:

1. Basic HTML document structure?
   Answer: <!DOCTYPE html><html><head><body> (Required semantic structure)

2. Purpose of <meta> viewport tag?
   Answer: Responsive design control (Controls viewport scaling on mobile)

3. Semantic element for navigation?
   Answer: <nav> (Defines navigation section)

4. Form submission methods?
   Answer: GET and POST (HTTP request methods)

5. Purpose of alt attribute?
   Answer: Image description (Accessibility and SEO)

6. HTML5 storage options?
   Answer: localStorage/sessionStorage (Client-side data storage)

7. Purpose of <article> tag?
   Answer: Independent content (Self-contained content)

8. Required form field attribute?
   Answer: required (Form validation)

9. Purpose of data-* attributes?
   Answer: Custom data storage (Store extra information)

10. HTML5 input types?
    Answer: email, number, date etc (Input validation)

11. Purpose of <aside> tag?
    Answer: Secondary content (Complementary content)

12. Form validation attributes?
    Answer: pattern, required, min/max (Client-side validation)

13. Purpose of <figure> tag?
    Answer: Self-contained content (Images with captions)

14. Semantic text elements?
    Answer: <strong>, <em>, <mark> (Text importance)

15. Audio/video attributes?
    Answer: controls, autoplay, loop (Media control)

16. Purpose of srcset?
    Answer: Responsive images (Different image sizes)

17. Form enctype values?
    Answer: multipart/form-data (File uploads)

18. Purpose of <main> tag?
    Answer: Main content (Primary content area)

19. HTML special characters?
    Answer: &lt; &gt; &amp; (Character encoding)

20. Canvas vs SVG?
    Answer: Pixel vs Vector (Graphics types)

21. Purpose of <time> tag?
    Answer: Date/time formatting (Machine-readable dates)

22. Form label connection?
    Answer: for attribute (Accessibility)

23. Purpose of <details> tag?
    Answer: Expandable details (Interactive disclosure)

24. Semantic table elements?
    Answer: <thead>, <tbody>, <tfoot> (Table structure)

25. Purpose of rel attribute?
    Answer: Link relationship (Link type definition)

26. HTML5 form validation?
    Answer: novalidate attribute (Disable validation)

27. Purpose of <picture> tag?
    Answer: Responsive images (Art direction)

28. Semantic list types?
    Answer: <ol>, <ul>, <dl> (List organization)

29. Purpose of <output> tag?
    Answer: Calculation results (Form calculations)

30. Meta charset purpose?
    Answer: Character encoding (Text encoding)

31. Purpose of <template> tag?
    Answer: Hidden content (Client-side templating)

32. Form method override?
    Answer: _method hidden field (RESTful forms)

33. Purpose of <progress> tag?
    Answer: Progress indication (Task completion)

34. Semantic grouping elements?
    Answer: <section>, <article>, <nav> (Content organization)

35. Purpose of manifest?
    Answer: Offline capabilities (PWA support)

CSS MCQs:

1. Box model components?
   Answer: Content, padding, border, margin (Layout structure)

2. Position values?
   Answer: static, relative, absolute, fixed (Element positioning)

3. Flexbox alignment?
   Answer: justify-content, align-items (Flex container alignment)

4. CSS Grid basics?
   Answer: grid-template-columns/rows (Grid layout)

5. Specificity calculation?
   Answer: ID > Class > Element (Selector priority)

6. Media query syntax?
   Answer: @media screen and (condition) (Responsive design)

7. CSS variables (custom properties)?
   Answer: --variable-name: value (Reusable values)

8. Transform functions?
   Answer: translate, rotate, scale (Element transformation)

9. Animation properties?
   Answer: @keyframes, animation (Motion design)

10. Display values?
    Answer: block, inline, flex, grid (Element rendering)

11. Box-sizing values?
    Answer: content-box, border-box (Size calculation)

12. Pseudo-classes?
    Answer: :hover, :focus, :active (State selectors)

13. Pseudo-elements?
    Answer: ::before, ::after (Generated content)

14. Float property?
    Answer: left, right, none (Element floating)

15. Clear property?
    Answer: left, right, both (Float clearing)

16. Transition properties?
    Answer: property, duration, timing (Smooth changes)

17. Background properties?
    Answer: color, image, position (Background styling)

18. Flexbox ordering?
    Answer: order property (Flex item order)

19. Grid template areas?
    Answer: grid-template-areas (Named grid areas)

20. CSS units?
    Answer: px, em, rem, vh/vw (Measurement units)

21. Overflow handling?
    Answer: visible, hidden, scroll (Content overflow)

22. Z-index stacking?
    Answer: Integer values (Layer ordering)

23. Filter functions?
    Answer: blur, brightness, contrast (Visual effects)

24. Column properties?
    Answer: column-count, column-gap (Multi-column layout)

25. Font properties?
    Answer: family, size, weight (Text styling)

26. List styling?
    Answer: list-style-type (List markers)

27. Border properties?
    Answer: width, style, color (Border styling)

28. Outline vs border?
    Answer: Outside border (Visual boundary)

29. Text decoration?
    Answer: underline, line-through (Text effects)

30. Viewport units?
    Answer: vh, vw (Responsive units)

31. Calc() function?
    Answer: Mathematical calculations (Dynamic values)

32. CSS counters?
    Answer: counter-increment (Automatic numbering)

33. Object-fit property?
    Answer: contain, cover (Image fitting)

34. CSS Grid gaps?
    Answer: grid-gap (Grid spacing)

35. CSS custom properties scope?
    Answer: :root scope (Global variables)

JavaScript MCQs:

1. Variable declaration methods?
   Answer: var, let, const (Scope differences)

2. == vs === operators?
   Answer: Type coercion vs strict equality (Comparison types)

3. Promise states?
   Answer: pending, fulfilled, rejected (Async states)

4. Arrow function syntax?
   Answer: () => {} (Concise functions)

5. Array methods?
   Answer: map, filter, reduce (Array operations)

6. Event bubbling?
   Answer: Bottom-up propagation (Event flow)

7. Closure definition?
   Answer: Function with preserved scope (Scope access)

8. this keyword context?
   Answer: Execution context (Object reference)

9. Prototype inheritance?
   Answer: Object prototype chain (Object inheritance)

10. Async/await purpose?
    Answer: Promise synchronization (Async handling)

11. Hoisting behavior?
    Answer: Declaration lifting (Variable/function declarations)

12. Destructuring syntax?
    Answer: {a, b} = obj (Value extraction)

13. Spread operator?
    Answer: ...array (Array/object expansion)

14. localStorage vs sessionStorage?
    Answer: Persistence difference (Storage duration)

15. Event delegation?
    Answer: Parent handling (Event optimization)

16. Map vs Object?
    Answer: Key types (Data structure)

17. Promise chaining?
    Answer: .then() chain (Sequential async)

18. Template literals?
    Answer: `${variable}` (String interpolation)

19. typeof operator?
    Answer: Type checking (Value type)

20. Array destructuring?
    Answer: [a, b] = array (Array unpacking)

21. Default parameters?
    Answer: function(x = 1) (Parameter defaults)

22. JSON methods?
    Answer: stringify, parse (Data conversion)

23. Class definition?
    Answer: class syntax (Object templates)

24. try/catch usage?
    Answer: Error handling (Exception handling)

25. setTimeout vs setInterval?
    Answer: Once vs repeated (Timing functions)

26. DOM manipulation?
    Answer: createElement, appendChild (DOM changes)

27. fetch API?
    Answer: Promise-based requests (HTTP requests)

28. Object.freeze()?
    Answer: Immutable objects (Object modification)

29. let vs const?
    Answer: Reassignment ability (Variable mutability)

30. Set data structure?
    Answer: Unique values (Collection type)

31. async function return?
    Answer: Always Promise (Async result)

32. Array.from() usage?
    Answer: Array conversion (Array creation)

33. Object methods?
    Answer: keys, values, entries (Object properties)

34. Generator functions?
    Answer: function* syntax (Iteratable functions)

35. Module syntax?
    Answer: import/export (Code organization)
