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
`php artisan nova:user`
`php artisan serve`

`http://127.0.0.1:8000/prescreening`
answers the questions

`http://127.0.0.1:8000/nova/resources/users/1`
notice `keyValue::make('answers')` doesn't work properly 

####location
https://github.com/kortby/key_value_issue/blob/main/app/Nova/User.php#L68