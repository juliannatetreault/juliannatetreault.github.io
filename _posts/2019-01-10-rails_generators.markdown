---
layout: post
title:      "Rails Generators"
date:       2019-01-10 17:17:28 +0000
permalink:  rails_generators
---


### What Rails Generators are

While they seem magical, Rails Generators are merely terminal commands that aid in the production of Rails applications. Rails Generators can be a helpful resource to have in your Rails toolbox, if used with discretion and at appropriate times.

There are four primary Rails Generators that can be used to assist in you in building your application, and a fifth generator that should be used sparingly. To begin, we’ll go over the four primary generators that are used more often by developers than the fifth generator. 
 
### What Rails Generators aren’t

A blessing and a curse, Rails Generators work best when they are used at an appropriate time. They are, in their most basic form, tools—tools that can be abused. Rails Generator abuse can occur from misuse and should be avoided at all cost. Generators are not a magical programming power that creates websites and saves lives—they are tools.

### When to use Rails Generators

Rails Generators work particularly well during the setup of the model-view-controller framework, or MVC for short. They give developers the ability to easily (and quickly) put together an MVC-based application, such as a CRUD application.

### How to use Rails Generators 

Rails Generators are surprisingly easy to use and implement in your future projects. All Rails Generator commands are done via your terminal. The command `rails generate`, or `rails g` for those keystroke-conscious developers, is the basis for each and every one of the Rails Generators. While the code that follows `rails g` changes depending on the type of generator you’re using, each generator command begins that same way.

### The five types of generators

* 1. Migrations
* 2. Models
* 3. Controllers
* 4. Resources
* 5. Scaffolding

#### Migration Generators

Migration Generators are utilized for creating quick and easy migrations. You can implement a Migration Generator by typing `rails g migration` followed by the name of the migration, or table you’re creating, followed by the column names and types. For example, creating a `Cats` table with a column for a cat’s breed would look something like this: 

`rails g migration CreateCats breed:string name:string age:integer`

#### Model Generators

Model generators are the bread and butter of generators. Used quite frequently, a Model Generator will create both the model and database table for the model. When generated, the model will automatically be set up to inherit from `ActiveRecord::Base`. To create a model and the model’s database table with the Rails Generator, use the following CLI command:

`rails g model Cat breed:string name:string age:integer`
 
#### Controller Generators

Controller Generators will, unsurprisingly, create a controller for the class of your choosing. Along with creating a generator, the Controller Generator command will also conveniently create routes for any of your generator arguments you pass to it, a directory full of corresponding view templates, a view helper method, and some styling files. If you wanted to create a controller and the above-mentioned corresponding routes, files, etc., you would use the following terminal command:

`rails g controller cat stats  cat_info owner_info`

#### Resource Generators

Resource Generators are great for creating most of the necessary structure needed for a MVC-based app. Using this command will create a database, a model and controller file that inherit from their appropriate bases, a view directory, a view helper file, a `resources` call in `routes.rb`, and some styling files. To use this command and generate these resources, type the following in your terminal:

`rails g resource Cat breed:string name:string age:integer`

#### Scaffolding Generator 

While simple to use, Scaffolding Generators should, for the most part, be avoided. What sets Scaffolding Generators apart from the rest is that they essentially build out every file you could need in a basic MVC project. This being said, Scaffolding Generators typically lead to unnecessary time wasted—there will be many useless resources created and you’ll have to spend time deleting said resources. Programmers are better off using one of the above generators instead, and then spend their time building out the resources they need, rather than spending it parsing and deleting. If you’re curious about Scaffolding Generators, you can generate one through the following CLI command: 

`rails g scaffold Cat breed:string name:string age:integer `

