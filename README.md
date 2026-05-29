# Pascal BCA 5th, .NET Technology - Lab Questions

## Notes for students
1. Please create your respository on https://github.com/Pascal-College-BCA-Fifth-2026, **Repository** name should be your `firstname-lastname`
2. There should be a folder for each question, which should contain your solution project and output snapshots.
3. For Quetion 1, you can have single project and implement all programs (1-7) there.
1. Generate final **PDF report** with all these solutions and snapshots you attached and  add it to the repo itself. You may want to use any AI tools for this job providing your repo as a context.

## Question 1 - Quick Programs  
1. Find Largest number among 3 numbers given?
1. Check if entered alphabet is vowel or not?
1. Check if entered number is even or not (use ternary operator)?
1. Calculate the sum of squares of first *n* natural numbers.
1. Write C# method that calculate average of 3 decimal number arguments.
1. Modify same method above that allows user to supply any number of argumnets and calculate average of all.
1. Wrtie C# method that count total males, females and others, given the array of genders as:
    ```csharp
    char?[] genderCollection = ['F', 'M', 'F', 'M', null, 'M', null, 'F', 'F', 'M', null, null, 'F', 'M', 'M' ];
    ```

## Question 2 - Create class named `*Collection*`, create 3 methods in there: 
1. `GetAnimals()` which returns array of animal names. 
2. `FetchSongs()` which returns list of songs (song name and genre).
3. `FetchSongs(bool includeArtist)` overload of (2). to return list of songs (name, genre and artist name).

Call all three methods from `Main()` and print results to console.

## Question 3 - Think of a real-world class within a proper namespace which should have:
1. Default and parameterized constructor
1. Two auto-implemented properties
1. A read-only property evaluated from other properties
1. An enumeraiton list within that namespace that this class genuinely need
1. A method `PrintDetails`, which displays all details of the object at console
1. In `Main()`, create objects of this class using both the constructors and call (5) for output in console

## Question 4 - Think of a scenario where you can design your classes as described below:
1. Base class 1 should have a method that can be overriden by child classes
1. Base class 1 should not allow its instantiation
1. Grand child should protect itself from getting inherited
1. Show case all the use-cases above in entry point

## Question 5 - Create a simple ASP.NET Core web app and ...
1. Add a new page **Counter** which should contain a HTML form with big textarea and submit button (Count).
1. Bu default textarea should contain following story text (*story* variable below) but user can enter their own paragrphs as well.
1. You should handle form submission as POST request.
1. When user submits form (hits Count button), user should be able to see following output in same page:
    > **Number of characters:** xxx

    > **Number of words:** xxx
    
    > **Number of sentences:** xxx
    
    > **Number of vowels:** xxx

    > **Number of special characters:** xxx

```csharp
var story = """
    Once upon a time, in a land far, far away, there lived a brave knight named Sir Lancelot. 
    He was known throughout the kingdom for his courage and chivalry. One day, he embarked on a 
    quest to rescue a princess from a fearsome dragon. With his trusty sword and unwavering determination, 
    Sir Lancelot faced the dragon in an epic battle. After a fierce fight, he emerged victorious and 
    saved the princess, earning the admiration of all who heard his tale.

    The grateful king rewarded Sir Lancelot with lands and treasures beyond measure. The princess, 
    impressed by his valor, soon fell in love with the noble knight. They were married in a grand 
    ceremony attended by lords and ladies from across the realm. Sir Lancelot and his beloved princess 
    lived happily ever after in a magnificent castle, where they ruled with wisdom and kindness. 
    Their legacy became the stuff of legend, inspiring generations of knights to pursue honor, 
    courage, and true love.    
""";
``` 

## Question 6 - Create MovieManager Web Portal
### Movie Mangaer have three related domain entities to deal with:
`Movie` (ID, Title, Rating, Budget, Gross, Release Date, Genre, Runtime, Summary)

`Actor`(ID, Name, Date of Birth, Birth City, Birth Country, Height (Inches), Biography, Gender, NetWorth)

`Charactor`(MovieID, ActorID, Character Name, Pay, Screentime)

### This app should have following features:
* Add new movies to database
* Add new actors to database
* Add new and update existing characters on database
* Dashboard page showing:
  * List of top 10 flop movies
  * List of top 5 highest paid actors and role they played

### Requirements
1. `ASP.NET Core` Razor Pages
1. Please use `SQLite` as your database
3. Use EF Core ORM tool for data access
