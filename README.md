g3server
========

G3Chat Server
1. Get the original openfire 3.7.1 source code from :http://olex.openlogic.com/packages/openfire/3.7.1
2. Merge the source code with G3Chat Server: https://github.com/coodeer/g3server
3. Install JDK and Ant tools for openfire build :http://apache.xmlcity.org/ant/binaries/
4. Build with Ant:
    Configure your JAVA_HOME and ANT_HOME, Enter openfire/build, run ant.
5. Build with Eclipse GUI.
  	a.  Read configure_openfire.pdf 
	b.  Merge the source code to original openfire 3.7.1 source code, build your xmpp server.
	c.  Open with eclipse(configure refer to configure_openfire.pdf)。
	d.  Install mysql in local for debug, and setup your database( run src/database/openfire_sqlserver.sql) to initialize the database[ I add a table ofG3ChatUser].
	e.  Run configure, then you can configure with http://127.0.0.1:9090  ,login with admin user, configure the database。
	f.  Configure the openfile( email setting for get password server)。
	g.  Run your g3chat client to connect with your local server。
	h.  If the debug is OK, build your project with ant. then you can get your target/openfire folder ( check the target/openfire/lib/openfire.jar was updated by ant and plugin was updated)
	i.  Upload your target/openfire folder to you really server, /bin/openfire.sh to run it( need configure with web again).
