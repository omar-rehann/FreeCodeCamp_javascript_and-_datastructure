# Student Grades Evaluator

This project is a simple JavaScript program that calculates a student’s grade, determines if they passed, and shows the class average.

## Features
- **getAverage(scores):** Calculates the average of all scores.
- **getGrade(score):** Returns the grade based on the score:
  - `A++` for 100
  - `A` for 90–99
  - `B` for 80–89
  - `C` for 70–79
  - `D` for 60–69
  - `F` for below 60
- **hasPassingGrade(score):** Checks if the student passed (not `"F"`).
- **studentMsg(totalScores, studentScore):** Returns a message including:
  - The class average
  - The student’s grade
  - Whether the student passed or failed

## Code Example

```js
function getAverage(scores) {
    let sum = 0;

    for (const score of scores) {
        sum += score;
    }

    return sum / scores.length;
}

function getGrade(score) {
    if (score === 100) {
        return "A++";
    } else if (score >= 90) {
        return "A";
    } else if (score >= 80) {
        return "B";
    } else if (score >= 70) {
        return "C";
    } else if (score >= 60) {
        return "D";
    } else {
        return "F";
    }
}

function hasPassingGrade(score) {
    return getGrade(score) !== "F";
}

function studentMsg(totalScores, studentScore) {
    const average = getAverage(totalScores);
    const grade = getGrade(studentScore);

    if (hasPassingGrade(studentScore)) {
        return "Class average: " + average.toFixed(2) + ". Your grade: " + grade + ". You passed the course.";
    } else {
        return "Class average: " + average.toFixed(2) + ". Your grade: " + grade + ". You failed the course.";
    }
}

console.log(studentMsg([92, 88, 12, 77, 57, 100, 67, 38, 97, 89], 37));
