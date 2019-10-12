# Item Catalog App

An application that provides a list of items within a variety of categories 
as well as provide a user registration and authentication system.
Registered users will have the ability to post, edit and delete their own items.

## More Further about project

 The Item Catalog project consists of developing an application that provides
 a list of items within a variety of categories, 
 as well as provide a user registration and authentication system.
 
 
## Dependencies

* [Vagrant](https://www.vagrantup.com/)
* [Udacity Vagrantfile](https://github.com/udacity/fullstack-nanodegree-vm)
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

## How to Install

1. Install Vagrant & VirtualBox
2. Clone the Udacity Vagrantfile
3. Go to Vagrant directory and either clone this repo or download and place zip here
3. Launch the Vagrant VM (`vagrant up`)
4. Log into Vagrant VM (`vagrant ssh`)
5. Navigate to `cd/vagrant` as instructed in terminal
6. The app imports requests which is not on this vm. Run sudo pip install requests
7. Setup application database `python database_setup.py`
8. Insert fake data `python database_init.py`
9. Run application using `python project.py`
10. Access the application locally using http://localhost:5000


## JSON Endpoints

* Restaurants JSON: `/restaurant/JSON`
> - Displays all Restaurants

* Restaurant Menu JSON: `/restaurant/<int:restaurant_id>/menu/JSON`
> - Displays Menus for a specific Restaurant
	
* Restaurant Menu JSON: `/restaurant/<int:restaurant_id>/menu/<int:menu_id>/JSON`
> - Displays a specific Restaurant Menu.
