# Data Uniformity Correction

> **Prompt:**
> "When processing user submitted data, often times when users input data they will misspell things, or use a first name instead of a whole name, or a last instead of a whole name, or they may include or omit a title like Mrs. or Colonel. Sometimes they may even input characters on accident due to typos, along with other confusing variations. This makes it difficult to make sense of the data due to the inconsistencies.
>
> Please provide me with a list of User Inputted Values, and after that a list of Expected Values, and I will associate each of the user inputted entries with the expected value. I will provide the output in a table format so it is easy for you to inspect the results to ensure that I have correctly associated the correct corresponding values. 
>
> Please provide the lists below:"

### User Inputted Values

| User Inputted Value |
|---------------------|
| John                |
| Smith               |
| Mr. John            |
| Jane                |
| Doe                 |
| Mrs. Jane           |
| Robert              |
| Johnson             |
| Dr. Johnson         |
| Amy                 |
| Cooper              |

### Expected Values

| Expected Value |
|----------------|
| John Smith     |
| Jane Doe       |
| Robert Johnson |
| Amy Cooper     |

### Associated Values

| User Inputted Value | Associated Value |
|---------------------|-----------------|
| John                | John Smith      |
| Smith               | John Smith      |
| Mr. John            | John Smith      |
| Jane                | Jane Doe        |
| Doe                 | Jane Doe        |
| Mrs. Jane           | Jane Doe        |
| Robert              | Robert Johnson  |
| Johnson             | Robert Johnson  |
| Dr. Johnson         | Robert Johnson  |
| Amy                 | Amy Cooper      |
| Cooper              | Amy Cooper      |
