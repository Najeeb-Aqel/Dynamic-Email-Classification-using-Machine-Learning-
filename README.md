
## About
More than 80% of data that companies collect about their customers is an unstructured data and
just very few of them make good use of it.
Emails are considered one of the biggest channels of unstructured data for companies, for some it’s the main tool to reach and interact with their customers, in this century we have seen new startups more than any time before with business models built around emails, such as email marketing, management, and email scripting.
More than twenty percent of user’s time is spent on email classification, unfortunately traditional classification techniques are usually primitive and un-flexible, leading to un-meaningful output that of no help for users.
In this project, a dynamic continuous refinement-approach has been taken to reach a more meaningful classification of emails that can truly give companies the advantage of being aware of their own environment, and willing take actions based on these new realizations.
The user will be given privilege to align the classification model based on their businesses’ needs and goals, through a direct interactive tool that will give the user broader perspective of both the human and the statistical parts of the data.

## In This Repo
This project has one main Python module `app.py` which runs the Flask application. A SQL database is created using the `database_setup.py` module and you can populate the database with test data using `database_init.py`.
The Flask application uses stored HTML templates in the tempaltes folder to build the front-end of the application. CSS/JS/Images are stored in the static directory.

## Skills & Libraries 
1. Python - Flask Framework 
2. HTML
3. CSS
4. OAuth
5. Flask Framework
6. Pandas 
7. Numpy 
8. Dash Framework 
9. LDA
10. Gensim


## Dependencies
- [Vagrant](https://www.vagrantup.com/)
- [Udacity Vagrantfile](https://github.com/udacity/fullstack-nanodegree-vm)
- [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## How to Install
1. Install Vagrant & VirtualBox
2. Clone the Udacity Vagrantfile
3. Go to Vagrant directory and either clone this repo or download and place zip here
3. Launch the Vagrant VM (`vagrant up`)
4. Log into Vagrant VM (`vagrant ssh`)
5. Navigate to `cd/vagrant` as instructed in terminal
6. The app imports requests which is not on this vm. Run sudo pip install requests
7. Setup application database `python /item-catalog/database_setup.py`
8. *Insert fake data `python /item-catalog/database_init.py`
9. Run application using `python /item-catalog/app.py`
10. Access the application locally using http://localhost:5000

*Optional step(s)


## JSON Endpoints 


Catalog JSON: `/catalog/JSON`
    - Displays the whole topics and all key words.

Categories JSON: `/catalog/categories/JSON`
    - Displays all Topics

Category Items JSON: `/catalog/<path:category_name>/items/JSON`
    - Displays items for a specific Topic 

Category Item JSON: `/catalog/<path:category_name>/<path:item_name>/JSON`
    - Displays a specific key word.
