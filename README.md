# Todo API
## Description
A RESTful Todo API built during my course lessons in Web Development Bootcamp by Colt Steele. I tweaked it a bit with the ability to add a description to your Todos instead of just a titular element.
# Languages Used
* Javascript(jQuery)
* HTML
* CSS
* Mongo

# Frameworks Used
* Express
* Node

## The Description Feature
In app.js(featured labeled as 'todoMessage')

>   var newTodo = $('<li class="task">'+todo.name +'<span class="delete">X</span><span class="taskMessage">'+todo.message +'</span>' +'</li>');

> function createTodo(){
> //send request to create new todo
> var usrInput = $('#todoInput').val();
> var usrMessage = $('#todoMessage').val();
> $.post('/api/todos',{name: usrInput, message: usrMessage})
> .then(function(newTodo){
>   $('#todoInput').val('');
>  $('#todoMessage').val('');
>   addTodo(newTodo);
> })
> .catch(function(err){
>  console.log(err);
> })
> }

