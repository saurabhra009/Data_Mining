# Data_Mining

**Steps to dwonlload CVAT in MAC OS:**

**Step1:**
Download Docker for Mac. Double-click Docker.dmg to open the installer, then drag Moby the whale to the Applications folder. Double-click Docker.app in the Applications folder to start Docker. More instructions can be found here.

**Step 2:**
There are several ways to install Git on a Mac. The easiest is probably to install the Xcode Command Line Tools. On Mavericks (10.9) or above you can do this simply by trying to run git from the Terminal the very first time.
 git --version
If you don’t have it installed already, it will prompt you to install it. More instructions can be found here.

**Step 3:** 
Download and install Google Chrome. It is the only browser which is supported by CVAT.

**Step 4:**
Open a terminal window. The terminal app is in the Utilities folder in Applications. To open it, either open your Applications folder, then open Utilities and double-click on Terminal, or press Command - spacebar to launch Spotlight and type “Terminal,” then double-click the search result.

**Step 5:**
Clone CVAT source code from the GitHub repository with Git.

The following command will clone the latest develop branch:

git clone https://github.com/opencv/cvat
cd cvat

**Step 6:**
Run docker containers. It will take some time to download the latest CVAT release and other required images like postgres, redis, etc. from DockerHub and create containers.
docker-compose up -d

**Step 7:**
(Optional) Use CVAT_VERSION environment variable to specify the version of CVAT you want to install specific version (e.g v2.1.0, dev). Default behavior: dev images will be pulled for develop branch, and corresponding release images for release versions.

CVAT_VERSION=dev docker-compose up -d

**Step 8:**
You can register a user but by default it will not have rights even to view list of tasks. Thus you should create a superuser. A superuser can use an admin panel to assign correct groups to other users. Please use the command below:

docker exec -it cvat_server bash -ic 'python3 ~/manage.py createsuperuser'

Choose a username and a password for your admin account when prompted.

Above command line will successfully create username and password to login in to the chrome for cvat.

**Step 9:**

Open the installed Google Chrome browser and go to localhost:8080. Type your login/password for the superuser on the login page and press the Login button. Now you should be able to create a new annotation task. 


**Screenshot of Login Screen of CVAT:**

<img width="1440" alt="01" src="https://user-images.githubusercontent.com/116526268/197423608-f3a924bd-322f-4ff3-a94d-d785f6a0123c.png">

**Screen after Login :**
<img width="1440" alt="02" src="https://user-images.githubusercontent.com/116526268/197423620-b6cc418e-6257-4c79-add9-356d979d520a.png">






