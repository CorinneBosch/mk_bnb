MakersBnb Web App
==================

```
                                          `'::::.
                                           _____A_
               x                          /      /\
    .-. _______|        /\-\           __/__/\__/  \___
----|=|/     /  \------_||"|_----------/__|" '' "| /___/\----
    | |_____|_""_|    ~^~^~^~^        |''|"'||'"| |' '||
    |_|_[X]_|____|                    `""`""))""`"`""""`
```
______

[Set up](#Setup) | [DB Connection](#DB) | [Interact](#Interact) | [Run Tests](#Tests) | [User Stories](#User-Stories) 

Team "Partially blind and computer less" present our very own MakersBnb clone.\
A collaboration between [Nicola](https://github.com/Nicola-Carroll), [Corinne](https://github.com/CorinneBosch) & [William](https://github.com/Willinlondon)


## Airbnb Clone
Our first group project at Makers Academy, learning and implementing the following techniques

- Introduction to Active Record
- Agile Methology for user stories & domain modeling
- Feature and Unit testing
- GET / POST requests - defining routes
- Creating Tickets & using Trello

Goals:
- Break down projects into tasks and allocate them to pairs
- Build to a specification (rather than challenges)
- Run stand-ups and retrospectives
- Use a branch/PR/merge git workflow
- Give and receive meaningful code review

## <a name="Setup">Set up</a>

1. **Fork** this [Bookmarker repository](https://github.com/CorinneBosch/Bookmarker/) 
2. Then clone **your** fork to your computer.
3. Ensure you have `Ruby` and `rspec` installed. Check ruby version with `ruby -v`
4. Install bundler if you haven't already. `gem install bundler`
5. Install the gems required by this repository. `bundle install`

## <a name="DB">DB Connection</a>

Before running the application on localhost, please migrate the database.\
If you wish to seed your db you can do so with the 2nd command.
```
rake db:migrate
rake db:seed
```

## <a name="Interact">Interact with the programme</a>

Open the application in your directory with `rackup`

Direct in your browser to `http://localhost:9292`.\
Now you can register on MakersBnb and browse through all the lovely listings!

You can frature test and run the makersbnb program in any `code editor` or `IRB`. 

## <a name="Tests">Run tests</a>

To test all units and features at once in your terminal.\
Print out the format documentation with the -fd shortcut.
```
$ rspec
$ rspec -fd
```

To test inividual unit or feature tests in your terminal:
```
$ rspec spec/units/user_spec.rb -fd
$ rspec spec/features/sign_in_spec.rb -fd
```

## <a name="User-Stories">User Stories</a>
Based on the objectives and expectations of our app we came up with the following user stories:

```
1. Any signed-up user can list a new space.
As a home owner
I would like to list my spare room on MK BnB
That I can earn some extra money

2. Users can list multiple spaces.
As a home owner
I would like to list multiple spare rooms on MK BnB
That I can earn some extra money

3. Users should be able to name their space, provide a short description of the space, and a price per night.
As a home owner
So that I can advertise my spare room
I want to be able to name, describe and set a pice for my room. (plus picture)

4. Users should be able to offer a range of dates where their space is available.
As a home owner
So that I can advertise my spare room
I want to be able to set an available date range to book my room.

5. Any signed-up user can request to hire any space for one night.
As a tenant
So that I can book a lovely trip
I would like to make a booking request on MK bnb.

6. Until a user has confirmed a booking request, that space can still be booked for that night.
7. Get approved by the user that owns that space.
As a home owner
That  can rent my room
I would like to approve a potential tenant to rent my room.

8. Nights for which a space has already been booked should not be available for users to book that space.
As a tenant
That I can avoid booking an unavailable room
I would like to only see available rooms
```

Source of challege requirements: [Makersacadeny - GitHub](https://github.com/makersacademy/course/tree/main/makersbnb)
