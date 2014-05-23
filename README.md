db2admintools
=============

This project provides a set of scripts to ease the database administration.

These files do not need installation, you can execute them directly. Some enviroment
variable could be defined in order to modify the default behaviour.

# FILES 

 * db2env
   * It helps to change the configuration easily when switching instances. It
     was based on OraEnv.
   * You should run this script by preceding the command with dot space (. ./db2env)
     in order to modify the current profile.
   * By default it reads db2greg db2greg file from /opt/ibm/db2/v10.5 installation.
   * To overide default behavior, define the DB2_DIR with th installation directory.
   * As advise, define the DB2_DIR variable in the .profile or .bashrc.
 * db2dirs
   * Lists the databases (alias) and nodes for each instance in a given server.
   * By default it reads db2greg db2greg file from /opt/ibm/db2/v10.5 installation.
   * To overide default behavior, define the DB2_DIR with th installation directory.
   * As advise, define the DB2_DIR variable in the .profile or .bashrc.
 * db2cksec
   * Checks the local security of DB2, by regarding the authorities (group) for the
     instances, and then connecting to each database and retrieving the authorities
     at database level.
   * By default it reads db2greg db2greg file from /opt/ibm/db2/v10.5 installation.
   * To overide default behavior, define the DB2_DIR with th installation directory.
   * As advise, define the DB2_DIR variable in the .profile or .bashrc.
 * db2chdirs
   * Attaches to any remote node, and tries a connection to any local and remote
     database.
   * Even if the connection or attachment is not successful because of the
     password, it allows to detect invalid catalogations.
   * By default it reads db2greg db2greg file from /opt/ibm/db2/v10.5 installation.
   * To overide default behavior, define the DB2_DIR with th installation directory.
   * As advise, define the DB2_DIR variable in the .profile or .bashrc.

