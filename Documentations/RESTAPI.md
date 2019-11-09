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

## Subject

## Exam 

## Marks
