- Searching Some APIs for Quiz.
- Drop the Plan of API's for Quiz. Sticking with the database and Custom Quiz.

```sql
CREATE TABLE Quizzes (
    QuizID INT AUTO_INCREMENT PRIMARY KEY,
    Title VARCHAR(255) NOT NULL,
    Description TEXT,
    CategoryID INT,
    CreatorUserID INT,
    CreationDate TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
    FOREIGN KEY (CategoryID) REFERENCES Categories(CategoryID),
    FOREIGN KEY (CreatorUserID) REFERENCES Users(UserID)
);
```
- try out [Chart.js](https://www.chartjs.org/) To Create Chart For LeaderBoard.
