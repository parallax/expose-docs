#Change Log


- [Version Structure](#structure)
- [Pending Release](#pending)
- [5.5.1](#5.5.1)
- [5.4.1](#5.4.1)

<a name="structure"></a>
### Version Structure

*   5.4 = current laravel version
*   1 = expose version
*   0 = change within expose version




<a name="pending"></a>
### Pending Release


*   NEW FEATURE: Added in new `pixel_url` helper function that will allow you to generate a valid pixel image URL with ability to pass width and height to generate a quick resized image
*   Updated to make `?redirect=/something` work when you are sent to admin login and returns the user to the set page after they successfully login
*   Bugfix - Make sure image editable link has a value before putting link tag around image.
*   Added auto upgrade script ready for 5.5 release.


<a name="5.5.1"></a>
### 5.5.1.* <larecipe-badge type="success">Latest</larecipe-badge>



This set of versions support Laravel 5.5

<a name="5.4.1"></a>
### 5.4.1.*

> {warning} This version will stop being worked on once full 5.5 version is released and sites migrated.

This set of versions support Laravel 5.4


5.4.1.17
--------

*   Updated sidebar documentation to switch based on text processor driver. E.g. markdown or textile.

5.4.1.16
--------

*   Updates to fix email notification when a new user is created
    
*   Bugfix to correct issues around GTM and analytics tracking codes not showing
    
*   Bugfix to remove deleted\_at from showing within the advanced admin area to avoid updates making things incorrectly as deleted.
*   Added ability to put a css class on the body tag
*   Updated advanced admin dashboard to open direct page links rather than admin page management area
*   NEW FEATURE: Video embed editable that lets you easily embed a Youtube of Vimeo URL to an iframe
*   NEW FEATURE: hold shift key to highlight all available editables
*   NEW FEATURE: hold alt key when clicking on a link editable to follow the link set
*   NEW FEATURE: Admin area to manage and dynamically generate sitemap.xml based on conditional rules that the admin has control over view interface
*   Updated to add support for admin redirect on Kubernetes sites

5.4.1.15
--------

*   Bugfix to change the name of the expose svg blade directive to exposeSvg as clashes with other blade package helpers.
*   Added soft deletes to be used for pages to avoid issues when deleting related content that is attached to a page

5.4.1.14
--------

*   Updated to add ability to pass an order by and order dir option for sidebar relationships.
*   Updated to allowed name of related data to be overridden with getAdminNameAttribute in origin model

5.4.1.13
--------

*   Quick bugfix to make advanced record tables order by the first column by default

5.4.1.12
--------

*   Updates to advanced area and managable trait to allow more flexibility around registering different types of relationships.
*   Bugfix to managable trait to fix listable fields to be shown correctly.

5.4.1.11
--------

*   Added extra method to file editables to be able to get resolved full URL of the uploaded file with `->path()`

5.4.1.10
--------

*   Added new parameter to the text editable after default text to allow you to change the html tag that the editable is wrapped in. Default is a div, but you can pass in 'span' if needed. This is to help when editable is used within a styled up paragraph tag to allow it to sit within as it should. This may change to a default of span later once every site has been checked.

5.4.1.9
-------

*   Update to include nategood/httpful package which is need for HipChat helper functions.
*   Added new `AdminLoginRedirect` middleware to auto redirect a user if not logged in to the expose login page.
*   Added robots.txt helper to auto generate and handle difference between environments and exposecms.com domains

5.4.1.8
-------

*   New `php artisan env:push` and `php artisan env:fetch` commands added for use of centralised `.env.` management.
*   Added tracking of IP address when logging into expose auth micro service.
*   New Relic name corrected to remove laravel prefix and just use site name.
*   Bugfix to logo style in sidebar when site has global image tag styles set
*   Updated expose logo to be 2x for retina.

5.4.1.7
-------

*   **NEW** auth micro service released in to expose login system to create a centralised user management system with LDAP and 2 step auth. See docs for more information: [http://docs.exposecms.com/docs/laravel-services-auth-micro-service](http://docs.exposecms.com/docs/laravel-services-auth-micro-service)

5.4.1.6
-------

*   Trial run through QA of micro auth service for users

5.4.1.5
-------

*   Update to Expose Vzzar package to be included in latest expose package.

5.4.1.4
-------

*   Bugfix - Change to https detection follow changes to CloudFront headers being passed with new ALBs in place on sites.

Previous releases
-----------------

Anything prior to **5.4.1** is not tracked as this was still pre-beta phase and made for Laravel 5.2. For full information please review commit history of the repository