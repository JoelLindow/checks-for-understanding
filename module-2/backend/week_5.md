1. How do we make flash messages display on a page?
- By assigning a message to the "flash hash". These messages can be set to render in a view when  the message is set in the controller.

2. Where is cart information/temporary information usually stored?
- Within the session

3. What might be some reasons not to store cart in our database? Are there any reasons why we would want to persist that information?
- For a user that is not logged in yet.
- For an cart that might never become an actual processed order. We would not want to persist that data becasue it could potentially pervert our data on actual orders, sa well as clog up the database with irrelevant data.

4. What is the purpose of the asset pipeline?
- To allow large amounts of files that help populate our page properly to be compressed and compiled into 1 single file that can be transfered and read simply by machines receiving the information.

5. Why do we precompile our assets?
- Kill Whitespace
- Compile data to a large single straing for transfer

6. What do each of the following tags do?

```ruby 
<%= stylesheet_link_tag "application" %>
```
* Allow access to the CSS (cascading style sheets) for the application.
```
<%= javascript_include_tag "application" %>
```
* Allow access to the JavaScript scripts for the application.
```
<%= image_tag "rails.png" %>
```
* This is an example of using an ERB tag as an "image helper tag". 

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?
* Information on the Gem File
* Images that showcase the usage of the application
* Instructions on Database creation and seeding
* Known Issues
* Ways others would be invited to contribute

8. What are the top four accessibility issues that we as developers should be aware of?
* Color Blindness
* Poor vision
* Cognetive limitations
* Language Barriers

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?
* A callback.

10. Given the following object, how would we create a scope for all users who are active?
```ruby 

User.create(name: "Happy", active: true)
```
* ??? I'm not sure. I don't understand the question.

11. What is the difference between a scope and a class method?

* I'm still trying to figure that out. I would like to see this comcept covered in its simplets form to understand it better.
