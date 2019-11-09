# RMS REST APIs

## Base URL
```

```

##  School

- Get all schools   
```
GET - /schools
```

- Get school
```
GET - /schools/{schoolId}
```

- Create school
```
POST - /schools

Body:
{
  "name": "schoolName",
  "address": "address"
}
```

- Delete a school 
```
DELETE - /schools/{schoolId}
```


##  Semester

- Get all semesters   
```
GET - /schools/{schoolId}/semesters
```

- Get semester
```
GET - /schools/{schoolId}/semesters/{semesterId}
```

- Create semsester
```
POST - //schools/{schoolId}/semesters

Body:
{
    "id": 1,
    "name": "Test",
    "annualYear": "2019/20",
    "startDate": "2019-04-01",
    "endDate": "2019-03-31",
    "isActive": true,
    "schoolId": 1
}
```

- Delete a semester 
```
DELETE - /schools/{schoolId}/semesters/{semesterId}
```

##  Batch (Class)


- Get all batches   
```
GET - /schools/{schoolId}/batches
```

- Get batch
```
GET - /schools/{schoolId}/batches/{batchId}
```

- Create batch
```
POST - //schools/{schoolId}/batches

Body:
{
    "id": 1,
    "schoolId": 1,
    "className": "test",
    "isActive": false
}
```

- Delete a batch 
```
DELETE - /schools/{schoolId}/batches/{batchId}
```

## Student

- Get all students   
```
GET - /schools/{schoolId}/batches/{batchId}/students
```

- Get student
```
GET - /schools/{schoolId}/batches/{batchId}/students/{studentId}
```

- Create student
```
POST - /schools/{schoolId}/batches/{batchId}/students

Body:
{
    "id": 1,
    "name": "Test",
    "birthDate": null,
    "address": null,
    "email": null,
    "nationality": null,
    "enrollmentDate": null,
    "zipCode": null,
    "city": null,
    "state": null,
    "country": null,
    "schoolId": 1,
    "batchId": 1,
    "mobileNumber": null,
    "gender": null
}
```

- Delete a student 
```
DELETE - /schools/{schoolId}/batches/{batchId}/students/{studentId}
```

## Subject

- Get all subjects   
```
GET - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/subjects
```

- Get subject
```
GET - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/subjects/{subjectId}
```

- Create subject
```
POST - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/subjects

Body:
{
    "id": 1,
    "name": "Test",
    "description": null,
    "schoolId": 1,
    "semesterId": 1,
    "batchId": 1
}
```

- Delete a subject 
```
DELETE - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/subjects/{subjectId}
```

## Exam 

- Get all exams   
```
GET - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/exams
```

- Get exam
```
GET - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/exams/{examId}
```

- Create exam
```
POST - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/exams

Body:
{
    "id": 1,
    "name": "Test",
    "totalMarks": 100,
    "schoolId": 1,
    "semesterId": 1,
    "batchId": 1
}
```

- Delete a exam 
```
DELETE - /schools/{schoolId}/semesters/{semesterId}/batches/{batchId}/exams/{examId}
```

## Marks
