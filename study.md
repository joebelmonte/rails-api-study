# Rails as an API Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [Rails API Template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   Better Explained
    -   [Starting Ruby on Rails: What I Wish I Knew](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
        (sections 3 and 4)
    -   [Intermediate Rails: Understanding Models, Views and Controllers](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
        (up to and including "Quick Controllers")
-   Ruby on Rails Guides
    -   [Rails Routing from the Outside](http://guides.rubyonrails.org/routing.html)
        (up to and including chapter 2.6)
    -   [Action Controller Overview](http://guides.rubyonrails.org/action_controller_overview.html)
        (up to and including chapter 4.5)
    -   [The Rails Command Line](http://guides.rubyonrails.org/command_line.html)
        (up to and including chapter 1.4)

## Additional Resources

-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)

## Define Model Responsibilities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
They are classes that talk to the database.
```

## Define Controller Responsibilities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
They take input from the user and decide what to do with it.
```

## Define Router Responsibilities

In your own words, define what the router does in Rails.

```md
It recognizes URLs and dispatches them to a controller's action.  When necessary,
it can generate paths and URLS so that you don't have to on your own.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
- The web server receives the request, then finds which controller to use.
- The web server uses the dispatcher to create a new controller, call the action, and
  pass the parameters.
- The controller parses the request/data submittion/cookies, etc.
- It makes the appropriate request from the model for data.
- The View generates HTML, CSS, XML, JavaScript, and JSON using data given to it by the controller.
- The controller returns the response to the server.
- The server combines the data into an HTTP response and sends it to the user.
```
