There are 2 components in this application.
1. UserAccessManagement- Server side C# .Net MVC Web API project which contains all the API methods.
2. UserManagementApp- Client side Angular 6 project.

Steps to setup the application;
1. Run the POCScript.sql in Sql server Management studio to create the database.
2. Run the web api services by running the UserAccessManagement project.
3. Login to the application using the user
Username:Niranjan
password:123

/** A brief summary of the api methods called from the client side **/
GroupController : Group related api methods
  >> AddGroup -  Method for adding group
  >> GetGroupbyId - Method to get group by ID
  >> GetGroups - Method to get groups
  >> IsGroupExist - Method to check if group exists or not

LoginController : Login related api methods
  >> GetUserbyLoginName - Method to get user details by login name

RoleController : Role related api methods
  >> AddRole - Method to add Role
  >> GetRolebyId - Method to get role by id
  >> GetRoles - Method to get roles
  >> IsRoleExist - Method to check role exists

RoleGroupMappingController : Role and group mapping related api methods
  >> GetRoleGroupByRoleId - Method to get role by groupid
  >> GetRoleGroupNameByRoleId - Method to get group name by id
  >> GetUserbyRoleidGroupid - Method to get user by role and group
  >> AddupdateRoleGroup - Method to update role group

UserController : User related api methods
  >> AddUser - Method to add user
  >> GetUserbyId - Method to get user by id
  >> GetUsers - Method to get users
  >> IsUserExist - Method to check login exists

UserRoleGroupMappingController : Api methods related to Role and group assignment to the user
  >> GetUserRoles -  Method to get user roles
  >> AddUpdateUserRoleGroupMapping - Method to add user role group
  >> GetuserRoleGroupNamebyUseridRoleId - Method to get user role group by user id role id
  >> GetUserRoleGroupAssignByUserId - Method to get user role group by userid


