## Laravel nova 4 issue where KeyValue is not displaying all the data
```
KeyValue::make('Tenant Answers', 'answers')
->keyLabel('Answers')
->valueLabel('Questions')
->rules('json')
->hideFromIndex()
->readonly(true),
```
Key value is not displaying all the 15 questions/answers that I have in mysql database it does displays only 5 or 6 some times only 2 with NO Errors

## Question:
How can I be able to display all the json data?


## Setup

`php artisan migrate:fresh --seed`