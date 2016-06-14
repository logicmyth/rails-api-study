# Rails as an API Study

Use your favorite search engine and the provided readings to research and answer
the following questions (no prior knowledge is expected).

In your answers, be sure to cite any relevant sources you consulted in your
search. We ask you to write answers in your own words in order to see how you
process what you've read. Please do not answer with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [rails-api-template](/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   [Starting Ruby on Rails: What I Wish I Knew | BetterExplained](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
-   [Intermediate Rails: Understanding Models, Views and Controllers | BetterExplained](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)
-   [The Rails Command Line — Ruby on Rails Guides](http://guides.rubyonrails.org/command_line.html)
-   [Rails Routing from the Outside In — Ruby on Rails Guides](http://guides.rubyonrails.org/routing.html)
-   [Action Controller Overview — Ruby on Rails Guides](http://guides.rubyonrails.org/action_controller_overview.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
Models talk to the server. They store and validate data. I suppose their like a chef, or any producer, that gets orders from the controller and talk to someone to get the ingrediants and then produce the order. -betterexplained```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The controller relegates tasks to the model. It gives orders to the model and gives the model's info to the view. -betterexplained```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
A router gives a URL that the controller can boss the model about. It also does some coding for the programmer in that it performs paths and URLs so the programmer doesn't have to do it.  -guides.rails```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
The lovely client puts in a GET and the server the browser is on gives it to the router. The router gives the URL objective to the controller which gives a more specific action than GET, depending on the URL content, to the model. The model turns "0's and 1's" into something the compenents of the cycle and the programmer can work with. That goes to the controller which goes to the view and back to the client and the controller takes all the credit. -betterexplained```
