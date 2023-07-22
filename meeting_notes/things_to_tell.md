### Things I've found out this week
#### 22 July 2023
Helpful SQL Command to join output from two tables, without a JOIN or MERGE, also makes use of aliases:
```
SELECT E.F_NAME, E.L_NAME, D.DEP_NAME  
FROM EMPLOYEES AS E, DEPARTMENTS AS D 
WHERE E.DEP_ID = D.DEPT_ID_DEP
ORDER BY DEP_NAME, E.L_NAME DESC;
```
SQL Command to get average salaries by department
```
SELECT DEP_ID AS DEPARTMENT_ID, COUNT(DEP_ID) AS COUNT_IN_DEPT, AVG(SALARY) AS AVG_SALARY FROM EMPLOYEES GROUP BY DEP_ID;
```

#### 9 July 2023
- if you create a pandas dataframe and it contains a nested json, you can create 
  multiple columns using df.json_
  - In this example, a df made from results had a column which had a dictionary:
    ```
    data = requests.get(some_url)
    results = json.loads(data.text)
    df2 = pd.json_normalize(results)
    ```
- [List of Public APIs](https://github.com/public-apis/public-apis)
- Reacquainted myself with BeautifulSoup [help page](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)


#### 8 July 2023

I really need to keep better track of my learning, so I'll attempt to keep some notes in here.  I'm sure I'll modify things as I go, but this is a start.

This is most of what I looked into today.  I got the random user generator API from my course, then went down a rabbit hole trying to get a better way to keep some notes.

-  [Random user generator API](https://randomuser.me/)
- How to create GitHub Pages site and integrate with Jekyll
- How to use GitHub on my iPad 
  - lg2 command
  - alias git='lg2'

