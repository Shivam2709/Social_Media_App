# Social_Media_App

# Social Media Project

A social media project built using JavaScript, React.js, Node.js, MySql, and Express.js. that allows users to connect, share content, and interact with each other.

## Table of Contents
  - Introduction
  - Features
    a) User Authentication
    b) User Profiles
    c) Posts
    d) Social Interactions
    e) Privacy Settings
- Set up the database
- Tables
- Controllers
- routes
- Start the server and client

## Introduction

The social media project is a platform that enables users to create profiles, share posts, follow other users, like and comment on posts, and engage in various social interactions. 
The project aims to provide a user-friendly and intuitive social media experience.
The project should include features such as User Registration, User Profile, Post Creation, Likes and Comments and Dark Theme Light Theme functionalities. 
The user interface should be user-friendly and easy to navigate, with clear labels and intuitive icons.
The main purpose of this Project Enable users to create and publish posts with text Or images.

## Features

- User Authentication:
  - User registration and login
  - Password encryption and security

- User Profiles:
  - Create and customize user profiles
  - Update profile information and profile picture
  - View other users' profiles

- Posts:
  - Create, edit, and delete posts
  - Like and comment on posts
  - Share posts with other users

- Social Interactions:
  - Follow and unfollow other users

- Privacy Settings:
  - Control visibility of profile and posts


 Set up the database:
-I use SQL Database in this project

## Tables:
 - Comments
 - likes
 - posts
 - Relationships
 - user

## Controllers
- auth
- comments
- likes
- posts
- relationship
- user

## routes
- use("/api/auth", authRoutes)
     a) post("/login", login)
     b) post("/register", register)
     c) post("/logout", logout)
  
- use("/api/users", userRoutes)
        a) get("/find/:userId", getUser)
        b) put("/", updateUser)
  
- use("/api/posts", postRoutes)
       a) get("/", getPosts)
       b) post("/", addPost)
       c) delete("/:id", deletePost)
  
- use("/api/comments", commentRoutes)
      a) get("/", getComments)
      b) post("/", addComment)
      c) delete("/:id", deleteComment)
  
- use("/api/likes", likeRoutes)
     a) get("/", getLikes)
     b) post("/", addLike)
     c) delete("/", deleteLike)
  
app.use("/api/relationships", relationshipRoutes)
      a) get("/", getRelationships)
      b) post("/", addRelationship)
      c) delete("/", deleteRelationship)

# Start the server and client:
- In the `server` directory, run:
  ```
  npm start
  ```
- In the `client` directory, run:
  ```
  npm start
  ```
