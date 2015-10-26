Renewable Funding: Code Challenge
=================================

Hi there!  We're ecstatic that you're interested in working for Renewable Funding's dev team.  To get a better idea of your current development skills, we'd like for you to complete a code challenge - build an application according to a set of requirements.  The actual business requirements are listed further down, but here are the general tech requirements:

1. Write your code in Ruby.
1. Make sure your app is runnable on Mac OS X or Linux.
1. Do not require any for-pay software.
1. Include instructions for setting up and running your application.

Feel free to email us at [codechallenge@renewfinancial.com](codechallenge@renewfinancial.com) if you have any questions.

## Submission Instructions

1. Clone this repository.
1. Create (and switch to) a new branch in your local repository:

  ```bash
  % git checkout -b new-branch-name
  ```

1. Complete the project as described below within your local repository.
1. Create patches from your commits, and place them in a directory:

  ```bash
  % git format-patch master -o submission_patches
  ```

1. Create a .zip file with the contents of the patches directory:

  ```bash
  % zip -r submission_patches.zip submission_patches
  ```

1. Email the .zip file to [codechallenge@renewfinancial.com](codechallenge@renewfinancial.com), and put the position you are applying for in the email's subject.

If you have any questions about this submission process, feel free to email us.

#### Why can't I just fork, and submit a pull request?

Unfortunately, Github no longer allows you to fork a public repo and make it private, so your submission would be visible to the entire world.  We'd love to keep this fair and not give the last responders a possible unfair advantage (since they'd be able to see all prior submissions); hence the patch method.

## Project Description

Imagine that Renewable Funding has just acquired a new company, Dr. Deal-a-Day's "Deal a Day" (dot com).  Unfortunately, the company has never stored their data in a database, and instead uses a plain text file.  We need to create a way for the new subsidiary to import their data into a database.  Your task is to create a web interface that accepts file uploads, normalizes the data, and then stores it in a relational database.

Here are the business requirements:

1. Users must be able to upload (via an HTML form) a comma-separated values (CSV) file with the following columns: purchaser name, item description, item price, purchase quantity, merchant address, and merchant name.  You can assume the columns will always be in that order, that there will always be data in each column, and that there will always be a header line.  An example input file named `example_data.csv` is included in this repo.
1. Your app must parse uploaded files, normalize the data, and store the information in a relational database.
1. After upload, your application should display the total amount of revenue contained in the uploaded file.

If you're applying for either the **Senior Software Engineer**, **Software Architect**, or **Engineering Manager** position, there are two additional requirements:
* Users must log in with an email address and password.  User registration & authorization is not required; include instructions on how to log in with your submission.
* Non-logged in users should not have access to upload files. 

Your application does not need to:

* be written with any particular framework
* be aesthetically pleasing

#### Bonus options:

If you're feeling inspired, bonus points for:

* allowing a user to log in with their Github account
* also accepting tab-delimited files with no changes in the submission form

## Evaluation

Reviewers will assess your familiarity with standard libraries, and with object-oriented programming.

1. Did your application fulfill the basic requirements?
1. Did you document the method for setting up and running your application?
1. Did you follow the instructions for submission?
