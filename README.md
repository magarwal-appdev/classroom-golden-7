# Classroom

## Standard Workflow

 1. From [your Cloud9 repositories list](https://c9.io/account/repos), set up a workspace [as usual](https://guides.firstdraft.com/starting-on-a-project-in-cloud9).
 1. Set up the project: `bin/setup`
 1. Start the web server by clicking "Run Project".
 1. Navigate to your live application preview.
 1. As you work, remember to navigate to `/git` and **commit often as you work.**
 1. Make new branches freely to experiment! _Especially_ before starting on a new task.
 1. Run `rails grade` as often as you like to see how you are doing, but **make sure you test your app manually first to make sure it matches the target's behavior first**.
**If at any point `rails grade` or `rspec` fails with the message "Migrations are pending:**

Then open a Terminal prompt and run:

```
rails db:migrate RAILS_ENV=test
```

## Introduction

You'll start with an almost blank application that just has a navbar with links corresponding to each necessary resource.

This application has 2 database tables:

 - students (columns: first_name, last_name, email)
 - courses (columns: name)

Each resource needs 7 "golden" actions to allow users to interact with it:

### CREATE

 - new_form
 - create_row

### READ

 - index
 - show

### UPDATE

 - edit_form
 - update_row

### DELETE

 - destroy

Build the Golden Seven for Students and Courses from scratch, the same way that you did for Photogram Golden 7. Hint: [the README for Photogram Golden 7](https://github.com/appdev-projects/photogram-golden-7#photogram-golden-seven) will come in handy.

### [Here is your target.](https://classroom-target.herokuapp.com/)

Make yours work like it. Your local app is using a light theme, and the reference app is using a dark theme so that you don't get confused between tabs as you try to check your work.

If you run into any problems or error messages, **use the server log to help figure out what's going on.**

I've already generated both database tables and models for you, so you just have to do build the interface for users to CRUD records. All in all, you need to:

 - Build the Golden Seven for Students from scratch.
 - Build the Golden Seven for Courses from scratch.

Some tools that you've got:

 - You can use the `rails console`.
 - You can navigate to `/admin` to see the admin dashboard; sign in with username: `admin@example.com` and password: `password`.
 - When you ran `bin/setup`, it included a script to pre-populate both tables with some dummy data for you. You can see what's there using either `rails console` or the admin dashboard.

Again, [the README for Photogram Golden 7](https://github.com/appdev-projects/photogram-golden-7#photogram-golden-seven) will be a good guide to follow; the Golden 7 are pretty formulaic.
