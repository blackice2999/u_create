
===============================================================================

U Create module

Drupal 7.x compatible

===============================================================================

alex [at] developmentseed [dot] org
felix [at] delattre [dot] de

===============================================================================

Do you want to:

- have users who don't have access to admin/* pages create other users?
- have users who don't have access to admin/* pages block/unblock other users?
- have a really easy way to create a new user and send her a personal message
  along with with the account info?
- assign user particular roles on creation?
- do all this with or without organic groups?

Use U Create!

===============================================================================

WARNING:

Handle 'assign user roles' permission with extreme care.

Any user with the 'assign user roles' permission in addition to the
'create users' permission will be able to create users of any available role.
Depending on the site setup, granting this permission can pose a severe security
risk. Make sure it is only granted to roles for admin level users.

Drupal 7 will ship without the 'assign user roles' permission.

===============================================================================

Installation:

1. Enable the module on admin->build->modules

2. Grant user permissions "create user" to a certain role. Now they should have a menu item in the navigation to add users, even if they are not allowed to administer all users.

3. You can also assign the "block user" permission to a certain role. These users can block and activate users through tabs on the user profiles (even if they don't have permission to administer all users). This could be useful for moderators etc.

(The Ucreate OG module alters the add user form to assign the new user to a group. If the person that is adding a new user has the needed permissions for this group)

===============================================================================