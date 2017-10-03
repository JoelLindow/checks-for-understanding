## Week One - Module 3

Some of these questions are from this week, some are from previous weeks, and some are new concepts. Try answering without research first. If you are not sure, take a guess but acknowledge that it's a guess (faking an answer in an interview without acknowledging it as a guess is a bad idea). Follow up with the necessary research to understand these concepts. These tend to be common themes during the job hunt and are worth having a solid understanding of.

1. What is `json`, what does it stand for, and why is it important?
   * Java Script Object Notation. It's a data format that a lot of languages already have libraries built to be able to accept and talk to. 
   * Easy way to pass a lot of data as a string. Easy for machine reading and human reading. Can be easily mapped.
   
2. What kind of object is JSON in Ruby? How do we know it's JSON?
   * It is a string.
   * We know by looking at it. It's in quotes. We know it's JSON becasue of the syntax, which looks similar to a hash with extra line returns. 

3. What's an API?
   * Application Programing Interface
   * A way for applications to share or use information with eachother.
   
4. What's a RESTful API? How does that look in Rails?
   * An API that sticks to RESTful conventions. No custom routes. 
   * No custom actions in controllers
   * There's no real "spec" for it so there can be some gray area.

5. What is an ORM, what does it stand for, and why is it helpful?
   * A set of libraries/classes that lets tables talk to eachother. Can take relational data from tables and provides a map to allow those tables to talk to eachother. 
   * Object Relational Mapper
   
6. How do you create a record in the following table in SQL? In Active Record?   
   (Users table with columns first_name, last_name, email, and age)
   * SQL: INSERT INTO people (first_name, last_name, email, age) VALUES ("Jeffrey", "Lebowski", "thedude@hollywoodlanes.com", 42 )
   * ACTIVE_RECORD: .create(first_name: "Jeffrey", last_name: "Lebowski", email: "thedude@hollywoodlanes.com", age: 42) 
   
7. How would you refactor this method?

```
def people_with_brown_hair
  people_with_brown_hair = []

  people.each do |person|
    if person.hair_color == "brown"
      people_with_brown_hair << person
    end
  end

  people_with_brown_hair
end
```
* refactor

```
def people_with_brown_hair
  Person.where(hair_color: "brown")
end
```

8. Given an array numbers = [1,2,3,4,5], find the sum of the doubles of all the numbers.  
```
numbers = [1,2,3,4,5]
numbers.inject(0) { |sum, num| sum + (num * 2) }
```

#### Self Assessment  
Rate yourself on the following scale.  
3  I know and understand most of these concepts but had to look something up  
