# ToDoListApi
Api for todo list including database file

Host on an apache server and run the .sql file first 

the api can be accessed via the url : https://$domain_name/TodoController.php

the parameters are to be post variables sent as such
for add :
$_POST['todo_title'];
$_POST['todo_descr'];
$_POST['todo_time'];
adds the info returns a string indicating success or failure

for update :
$_POST['todo_id'];
$_POST['todo_title'];
$_POST['todo_descr'];
$_POST['todo_time'];
updates the row with the todo_id and returns a string indicating success or failure

for delete :
$_POST['todo_id'];
deletes the row with the todo_id and returns a string indicating success or failure


for view :
$_POST['todo_id'];
finds the row with the todo_id and returns a jsonArray containing it's record
