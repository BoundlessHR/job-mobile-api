# Mobile Test Project - Jobs App

Your task is to implement a simple Job Board mobile application using Ionic Framework. Detailed specifications for the test project are provided below. We estimate that you will not need more than a single weekend at relaxed coding speed to implement it.

## Project Description

The Job Board mobile application will be used by your Users (Job Seekers) to perform the following tasks:

- List Job Posts
- Filter Job Posts
- View a job post indivisually

## Technical details

You mobile application should be built on Ionic Framework, and consume Akhtaboot's public jobs API.

### Akhtaboot public jobs API

The public API supporst X actions:

- Index:

    url: `https://akhtaboot.com/api/v1/jobs` GET

    params: per_page, page, country, city, job_type, career_level, job_communities, _id

    send `?local=true` to retrieve your country jobs by your IP address

    You can get Jobs By ids by requesting the methods as the following

    `https://akhtaboot.com/api/v1/jobs?_id[]=job-44841&_id[]=job-44843`

- Show:

    Returns a single job's data

    url: `https://akhtaboot.com/api/v1/jobs/:job_id`

- Init:

    Returns a list of countries, cities, and communities

    url: `https://akhtaboot.com/api/v1/init`

- Create User:

    method: post

    url: `https://akhtaboot.com/api/v1/profiles/`

    params: email, password, password_confirmation, cv, doc


### Implementation

- Create an index page to list jobs.
- Add City & Country filter.
- Only list 10 jobs on the page, allow the user to view more.
- Add a show page for a single job listing it's details.
- Show job location on the map in the show page


### Bonus task (NOT mandatory)

- Implement more filters using the API.
- Allow users to signup.
- Implement search for Jobs by title or creation date.
- Allow users to signup and upload CVs through your application.

## Review process

There are a few technical restrictions so we can see how you fare with the technologies and processes we use on a daily basis, but in general, the actual implementation is quite open-ended. The reason is we want to see how you think in terms of architecture, development processes and how you generally deal with the challenges you might face while implementing this app.

The following should help you determine where to put your focus, since these are the things we will be looking for while reviewing your project.

### Testability

Is your code tested? How do you approach testing? Do you use TDD or are tests an afterthought for you.

### Validations and error handling

How do you handle required fields, and errors that might appear due to invalid data,
How do you handle responses and Exceptions

### Version Control

Please commit often and tell a story of your process with your commit history.

## Project Delivery

- source code delivery options:
    * Create a Fork of this repository on Bitbucket and then create a pull request back to it
    * Create a private repository on bitbucket and invite devteam@boundlessdrop.com
- Send us a functioning APK

> That's it. Good luck and we look forward to seeing your submission!
