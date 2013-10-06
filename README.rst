* Django based forum with moderated access and publishment process
==================================================================
- What we expect:

** Forum
=====

	* http://docs.django-cms.org/en/2.4.2/getting_started/configuration.html#cms-max-page-publish-reversions
	* http://docs.django-cms.org/en/2.4.2/getting_started/plugin_reference.html#inherit

** Gallery
=======

** Calendar
========

** That all under ACL/s
====================

	* http://docs.django-cms.org/en/2.4.2/getting_started/configuration.html#cms-public-for
	* http://docs.django-cms.org/en/2.4.2/getting_started/configuration.html#cms-permission

=====
* REF/s
=====
google-docs: dc-motylek (dm) - webovky
--------------------------------------

** auth
-----------
	* http://django-blog-zinnia.com/blog/2010/01 
        * https://docs.djangoproject.com/en/dev/topics/auth/ 


* INIT
=====
::
	dj-form$> git remote add origin git@github.com:pepe5/dj-form.git
	dj-form$> git push -u origin master

	* http://pragmaticstartup.wordpress.com/2012/06/26/django-guardian-a-full-access-control-logic-acl-example/

** django setup & maint.
------------------------------------------

	* cms uninstall apphooks (http://docs.django-cms.org/en/2.4.2/advanced/cli.html#cms-uninstall)

*** http://docs.django-cms.org/en/2.4.2/extending_cms/placeholders.html
Placeholders are special model fields that django CMS uses to render user-editable content (plugins) in templates. That is, it’s the place where a user can add text, video or any other plugin to a webpage, using either the normal Django admin interface or the so called frontend editing.

*** http://docs.django-cms.org/en/2.4.2/extending_cms/searchdocs.html
For powerful full-text search within the django CMS, we suggest using Haystack together with django-cms-search.

*** https://bitbucket.org/schinckel/django-menus#rst-header-tree-menu
An extension to django-mptt, this is a template that you can use to have a dynamic tree menu, where selecting items with children expands them, and selecting a leaf node follows the link. To use it, you'll need to have mptt installed into your project as well as this package.

*** http://blog.umlungu.co.uk/blog/2007/jul/29/simple-menu-django-flatpages/
first of all:
create one app::

        python manage.py startapp flat
        cd flat
        mkdir templatetags

create flatpage_menu.py and save
later go to templates dir

*** http://www.rossp.org/blog/2007/nov/27/menus/
::

      {% load menubuilder %}{% menu main %}
      {% for item in menuitems %} {{ item.title }} {% endfor %} 


** zinnia setup
----------------------
try::
	$> buildout ...
        
- - see file:~/opt/django-blog-zinnia-master/Makefile

it is::
        $> pip install djangorecipe
        $> pip install zc.buildout


Stu stashes
-----------------

	- file:~/text/dc_motylek/dc_motylek
	- file:~/tmp/djangocms1/djangocms1/
	- file:~/tmp/mezzanine-1
        - file:/mnt/lifeboat-tmp/=delta-sam7/=3pub-my-personal-only/py/django-blog-zinnia-master.zip
        - file:~/opt/stephenmcd-mezzanine-a1c36d7/README.rst
