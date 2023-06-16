This repsitory contains 3 jsonc files that is used to store, read, and transmit data between different systems or components.
1. soal_baca.jsonc : contains reading quizzes data
2. soal_hitung (1).jsonc : contains counting quizzes data
3. soal_tulis.jsonc : contains writting quizzes data
## soal_baca.jsonc
below is code snippet from **soal_baca.jsonc**
```
{
  "lessons": [
    {
      "lessonType": "baca",
      "lessonLevel": 100,
      "questions": [
        {
          "type": "baca_input_suara",
          "question": "A",
          "answer": ["a"],
          "tags": ["baca_a"]
        },
        {
          "type": "baca_input_suara",
          "question": "B",
          "answer": ["b"],
          "tags": ["baca_b"]
        },
        ...
      ]
    },
    ...
  ]
}
```

### Lesson Object
To represent a lesson.
```
"lessons": [
    {
      "lessonType": "baca",
      "lessonLevel": 100,
      "questions": [
        {
```
Properties : 
- **lessonType** (string): Indicates the type of lesson.
- **lessonLevel** (integer): Represents the level or difficulty of the lesson.
- **questions** (array): Contains an array of question objects for the lesson.

### Question Object
To represent a question within a lesson.
```
"questions": [
  {
    "type": "baca_input_suara",
    "question": "A",
    "answer": ["a"],
    "tags": ["baca_a"]
  },
```
Properties :
- **type** (string): Indicates the type of question.
- **question** (string): Represents the question or prompt.
- **answer** (array): Contains the correct answer(s) to the question.
- **tags** (array): An array of tags or labels associated with the question.
- **feedback_img** (string, optional): Path to the feedback image associated with the question.

## soal_hitung (1).jsonc
below is code snippet from **soal_hitung (1).jsonc**
```
{
  "lessons": [
    {
      "lessonType": "hitung",
      "lessonLevel": 100,
      "questions": [
        {
          "type": "tulis_soal_teks",
          "question": "0",
          "answer": ["0"],
          "tags": ["tulis_0"]
        },
        ...
      ]
    },
    ...
  ]
}
```

### Lesson Object
To represent a lesson
```
"lessons": [
    {
      "lessonType": "hitung",
      "lessonLevel": 100,
      "questions": [
```
Properties :
- **lessonType** (string): Indicates the type of lesson.
- **lessonLevel** (number): Represents the level or difficulty of the lesson.
- **questions** (array): Contains an array of question objects for the lesson.

### Question Object
To represent a question within a lesson.
```
"questions": [
  {
    "type": "tulis_soal_teks",
    "question": "0",
    "answer": ["0"],
    "tags": ["tulis_0"]
  },
```
Properties :
- **type** (string): The type of the question.
- **question** (string): The question text or description.
- **question_img** (string, optional): The URL of the question image.
- **answer** (array): An array of correct answer(s).
- **tags** (array): An array of tags or labels associated with the question.

## soal_tulis.jsonc
below is code snippet from **soal_tulis.jsonc**
```
{
  "lessons": [
    {
      "lessonType": "tulis",
      "lessonLevel": 100,
      "questions": [
        {
          "type": "tulis_soal_teks",
          "question": "A",
          "answer": ["A"],
          "tags": ["tulis_A"]
        },
        {
          "type": "tulis_soal_suara",
          "question": "A besar",
          "answer": ["A"],
          "tags": ["dikte_A"]
        },
        ...
      ]
    }
  ]
}
```

### Lesson Object
To represent a lesson
```
{
  "lessons": [
    {
      "lessonType": "tulis",
      "lessonLevel": 100,
      "questions": [
```
Properties :
- **lessonType** (string): Indicates the type of lesson.
- **lessonLevel** (integer): Represents the level or difficulty of the lesson.
- **questions** (array): Contains an array of question objects for the lesson.

### Question Object
To represent a question within a lesson.
```
"questions": [
    {
      "type": "tulis_soal_teks",
      "question": "A",
      "answer": ["A"],
      "tags": ["tulis_A"]
    },
```
Properties :
- **type** (string): Specifies the type of the question.
- **question** (string): The actual question or task.
- **answer** (array): An array of possible answers for the question.
- **tags** (array): Contains tags or labels associated with the question.
- **feedback_img** (string, optional): The path to the image providing feedback for the question (applicable for specific questions).
