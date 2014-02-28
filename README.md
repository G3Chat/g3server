g3server
========

G3Chat Server

1.  Read configure_openfire.pdf 
2.  Merge the source code to original openfire 3.7.1 source code, build your xmpp server.
3.  Open with eclipse(configure refer to configure_openfire.pdf)。
4.  Install mysql in local for debug, and setup your database( run src/database/openfire_sqlserver.sql) to initialize the database[ I add a table ofG3ChatUser].
5.  Run configure, then you can configure with http://127.0.0.1:9090  ,login with admin user, configure the database。
6.  Configure the openfile( email setting for get password server)。
7.  Run your g3chat client to connect with your local server。
8.  If the debug is OK, build your project with ant. then you can get your target/openfire folder ( check the target/openfire/lib/openfire.jar was updated by ant and plugin was updated)
9.  Upload your target/openfire folder to you really server, /bin/openfire.sh to run it( need configure with web again).
