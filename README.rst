* Django based forum with moderated access and publishment process
==================================================================
- What we expect:

** Forum
=====

	* http://docs.django-cms.org/en/2.4.2/getting_started/configuration.html#cms-max-page-publish-reversions
	* http://docs.django-cms.org/en/2.4.2/getting_started/plugin_reference.html#inherit

** Gallery
=======
try:
	* https://imagestore.readthedocs.org/en/latest/install.html
	* https://github.com/stefanfoulis/django-filer


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

*** django-cms-demo$> source env/bin/activate
	- w/prerq:django-cms-demo$> virtualenv env
	- is this equivalent for $> workon ..#?


** django setup & maint.
------------------------------------------

	* https://github.com/andrewschoen/django-cms-demo
        * http://ilian.i-n-i.org/tag/django-cms/
	* cms uninstall apphooks (http://docs.django-cms.org/en/2.4.2/advanced/cli.html#cms-uninstall)

*** 1st-own try: $> pip install django-cms django-blog-zinnia imagestore django-reversion django-menu django-tagging djangorecipe zc.buildout
	- prerq: virtualenv env && source env/bin/activate

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


*** try>! http://jsfiddle.net/Ne227/1/

	- found by: http://stackoverflow.com/questions/11587407/displaying-menu-on-hovering-over-item-in-list
::
	<ul id="nav">
        <li><a href="index.htm" title="Home">Home</a></li>
        <li><a href="project.htm" title="Project">Project</a></li>
        <li><a href="sample.htm" title="Sample">Sample</a>
        <ul id="dropdown">
            <li><img src="http://mi.eng.cam.ac.uk/research/projects/Query/img/arrow.png"/></li>
            <li>Dropdown1</li>
            <li>Dropdown2</li>
            <li>Dropdown3</li>
            </ul>   
        </li>
        </ul>

::
        #nav li{
            float: left;
            padding: 5px;
        }
        #dropdown {
            display: none;
        }

        #nav li:hover #dropdown{
            display: block;
            position: absolute;
        }

        #dropdown li {
            float: none;
        }

        img {
            width: 80px;
            height: 60px;
            position: absolute;
            top: 20px;
            left: -90px;
        }



*** https://groups.google.com/forum/#!msg/django-cms/SIliMe9RFf8/iHdL6EQiVCoJ
I am using Django/Django CMS and Ext 3.3.1 with the Superfish 1.4.8 javascript library to build drop down menus. The menu system works great in Firefox, but is more or less non-functional in IE. The top level menu entries are visible, and colors change while hovering over different choices, but they do not drop down in IE. I would appreciate if anyone has had experience with this, and can tell me where to start looking to achieve this basic functionality in IE.

- It should be like [[file:/usr/lib/python2.6/site-packages/cms/static/cms/wymeditor/skins/default/skin.css::dropdown menu]
- >? my css seems to be skipped at all !
- >! try Customize your app’s look and feel (https://docs.djangoproject.com/en/1.5/intro/tutorial06/)


*** :whatif: [[file:~/text/dc_motylek/install-try.con.log::/20 redirections exceeded/]]

	- >? isnt it by file:~/text/dc_motylek/dc_motylek/settings.py::gettext ?
        < - seems to be caused by missing /language=cs


** zinnia setup
----------------------
try::
	$> buildout ...
        
- - see file:~/opt/django-blog-zinnia-master/Makefile

it is::
        $> pip install djangorecipe
        $> pip install zc.buildout


43_time
------------

	* https://www.google.cz/?#q=startapp+docs.django-cms.org%2Fen%2F2.4.2


Stu stashes
-----------------

	- file:~/text/dc_motylek/dc_motylek
	- file:~/tmp/djangocms1/djangocms1/
	- file:~/tmp/mezzanine-1
        - file:/mnt/lifeboat-tmp/=delta-sam7/=3pub-my-personal-only/py/django-blog-zinnia-master.zip
        - file:~/opt/stephenmcd-mezzanine-a1c36d7/README.rst
