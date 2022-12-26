# EasyMVC

EasyMVC is a very simple but useful mvc framework for php. You can edit and develop projects as you wish.

# Settings
 * U need to customize  -> config/default.php. 
 * U need create your controller methods to -> app/models
 * U need create your controller methods to -> app/controllers
    # Conditions
      * Your controller file name and controller class name should be same. Example Main.php should has class named Main
      * Your controller class should inherit from base controller class. Like that; `class Main extend controller{}`
      * Your model file name and model class name should be same. Example Main.php should has class named Main
      * Your model class should inherit from base model class. Like that; `class MainModel extend model{}`
      
# Controller Inherits 

* `render(file,params = []) => render a view file from app/views folder.` file : view path in views folder, params = whatever u want
* ` model(file) => import a model file from models folder` file: model class path in models folder
* `importClass(path,class) => import third party classes from classes folder.  path: file path in classes folder, class: class name in file`

# System variables 

 * db : database object u can use like that `$this->db` then u can use pdo statements with this parameter
 
 # Extras
 
  * # Helper Class
    Helper Class has some spesific methods. U can check here config/helper.php. U can custimize or add new methods what ever you want to here.
    than u can use like that `helper::yourmethod()` in whatever u want
  * # Session Manager Class
    Session manager class include createSession, deleteSession, AllSessionDelete, isLogged merhods. U can check config/sessionManager. 
    u can use like that `sessionManager->createSession(["UserId" => ''])` in controller or `sessionManager::createSession(["UserId" => ''])` in whatever u want.
    
    
