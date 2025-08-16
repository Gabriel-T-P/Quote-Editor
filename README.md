# Turbo Rails Project --- Quote Editor

This project is a Ruby on Rails 7 application that implements a **quote
editor** with reactive features using **Turbo Rails**, as presented in
the free Hotrails tutorial.

## About the Tutorial

The **Turbo Rails** tutorial teaches how to use `turbo-rails` (a library
included by default in Rails 7) to build single-page-like applications
(SPA-like), with little to no custom JavaScript.

What is implemented:

-   A simple CRUD controller for the `Quote` model\
-   CSS organization with the BEM methodology\
-   **Turbo Drive** --- speeds up navigation by intercepting clicks and
    form submissions, turning them into AJAX requests\
-   **Turbo Frames** and **Turbo Streams** --- to split pages into
    independent components and provide real-time updates with Action
    Cable\
-   Flash messages with animations using Stimulus\
-   Handling of empty states and UI messages with Turbo\
-   Dynamic calculation of the quote total when items are added,
    updated, or removed

## Project Goal

This project replicates the **Turbo Rails** tutorial from Hotrails,
implementing a fully functional quote editor:

-   Allows creating, editing, and deleting **quotes**, **dates**, and
    **items**.\
-   When interacting with the application (for example, adding an item
    or editing a date), the interface updates without reloading the
    page, thanks to Turbo.\
-   The quote total is dynamically updated as items are managed.

## Getting Started

1.  Clone this repository.\

2.  In the Gemfile, make sure you are using the compatible version of
    `turbo-rails`:

    ``` ruby
    gem "turbo-rails", "~> 1.0"
    ```

3.  Run:

    ``` bash
    bundle install
    bin/setup
    bin/dev
    ```

    This will install dependencies, create the database, run migrations,
    and start the server with automatic asset compilation.\

4.  Go to `http://localhost:3000` and explore the quote editor.

------------------------------------------------------------------------

## Reference

Based on the **Turbo Rails Tutorial** available at
[Hotrails.dev](https://www.hotrails.dev/turbo-rails).
