<img width="1429" alt="Screenshot 2023-06-16 at 1 47 54 AM" src="https://github.com/Vishnu2707/Blog/assets/86302373/985db1b5-5faf-488b-9b43-4b8d6054b235">

# Blog
A web app created using Django for blogging.

Django Admin page handles the post creation and deletion part.

To make a commit with all the modifications to Git from VSCode

cd Project/

git init - To initialize the repo

git add -A

git commit -m "commit name"

git push origin new-branch
--------------------------------------------------------------------------------------------------------
Setup
Update the System

(To check the branch you can use "git branch")

sudo apt-get update
To get this repository, run the following command inside your git enabled terminal

git clone https://github.com/Vishnu2707/Blog.git
You will need django to be installed in you computer to run this app. Head over to https://www.djangoproject.com/download/ for the download guide

Download django usig pip

sudo apt install python3-pip -y

pip install django
pip install pillow
Once you have downloaded django, go to the cloned repo directory and run the following command

python3 manage.py makemigrations
This will create all the migrations file (database migrations)* if required!

Now, to apply this migrations run the following command

python3 manage.py migrate
One last step and then our Blog App will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user

python3 manage.py createsuperuser
That was pretty simple, right? Now let's make the App live. We just need to start the server by following command now.

python3 manage.py runserver
Once the server is hosted, head over to http://127.0.0.1:8000/Blog for the App.

Once Hosted on the EC2 instance in AWS, you will not be able to see the app using the link http://127.0.0.1:8000 since the port 8000 is not allowed, so make sure to edit the security groups of the instance and add the port 8000. Now you will need to use http://16.16.182.77:8000/ to view the BLOG APP - SCRIBBLE!

Note - AWS EC2 instance is only free for 12 months!
