 MVC-Notes


Quick notes from "What is Programming MVC?" by DevMarketer
https://www.youtube.com/watch?v=1IsL6g2ixak




MVC

Model View Controller
Paradigm - way of thinking 
way of processing info
Way of structuring information
1979


Not a framework, just a way of thinking, way of structuring web applications

Why popular? Used by so many popular frameworks
	ruby
	cakePHP
	Django
	laravel
	zen framework
	codeIgniter
	iOS
	Objective C, Mac applications

Frameworks implement a MVC structure, but MVC itself is not a framework

MVC will help understand where to put what in the framework

M.V.C. - requires all three elements (with a few caveats, but basically) 

M: Model

	


MVC

Model View Controller
Paradigm - way of thinking 
way of processing info
Way of structuring information
1979


Not a framework, just a way of thinking, way of structuring web applications

Why popular? Used by so many popular frameworks
	ruby
	cakePHP
	Django
	laravel
	zen framework
	codeIgniter
	iOS
	Objective C, Mac applications

Frameworks implement a MVC structure, but MVC itself is not a framework

MVC will help understand where to put what in the framework

M.V.C. - requires all three elements (with a few caveats, but basically) 

M: Model

	


MVC prevents us from repeating ourselves
	create a solid structure
	everything has it’s place, makes it easy to locate things.
	

CLIENT
Client - user - browsers
	client is processing/rendering HTML/CSS/JS (client-side languages)
	
Request goes to google’s servers 

SERVER
	server usually runs linux/windows (Wordpress and go daddy are linux)
	server is running server-side languages such as PHP/Ruby/Python

DATABASE:
DB (mySQL, PostSQL, NOSQL, MongoDb
	contains all storage
	relational or non-relational


MODEL:	
	Database
	adding or retrieving items from DB
	processing data from or to the database
	speaks only with the controller



VIEW:
	Client
	What the client sees.  
	old fashioned HTML/CSS
	Speaks only with the controller




CONTROLLER:
	Server
	Processes GET/POST/PUT/DESTROY requests
	All server-side logic
	The middle Man
		Takes Info from user
		processes info and talks tot he DB if needed
		receives info from DB
		speaks to View to explain presentation to the viewer

	controller - “man in charge” and “middleman”

	bulk of the logic in the controller


 CONTROLLER ROUTE PROCESSING:
	frameworks all have a route processor
	www.web.com/contact - goes to contact
	“this is where you send it”, because it needs to know which controller is in charge of processing this page
	if you go to search, there’s a search controller
	if going to contact, it’s a pages controller
	post controller
	Controller directs the client 
	form, get request, etc
	decides what to do - usually database
	
Controller says I need this from you ( model), sends it back to the controller, controller takes the info that is needed in order to complete the view, sends it over to the view. 


- Basically the same across frameworks. Controller is middleman, talks to the model, model sends info back to the controller but model never talks to the view. After the controller gets the information, then it tells the view what to do and the view never talks back to the controller.



View is then compiled and sent to the user
