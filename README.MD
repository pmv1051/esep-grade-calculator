# ESEP Grade Calculator

This library is a simple utility to calculate your grades from 3 categories of grades.

The default categories and weights are:
Assignment 50%
Exam 35$
Edday 15%

The default letter grade ranges are:
90 - 100 -> A
80 - 89 -> B
70 - 79 -> C
60 - 69 -> F
0 - 59 -> F


```go
gradeCalculator := NewGradeCalculator()

gradeCalculator.AddGrade("Hello World", 100, Assignment)
gradeCalculator.AddGrade("DSA Final", 100, Exam)
gradeCalculator.AddGrade("Cool Software", 100, Essay)

letter := gradeCalculator.GetFinalGrade() // "A"
```


Runtime requirements:
Golang 1.24+

Run unit tests:
```
cd grade_calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade_calculator/
go test -coverprofile=coverage.txt ./...
```