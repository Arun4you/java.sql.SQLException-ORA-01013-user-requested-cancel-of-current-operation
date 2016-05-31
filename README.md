# java.sql.SQLException-ORA-01013-user-requested-cancel-of-current-operation



StatementTimeout relies on underlying JDBC driver support.

Weblogic Server passes the time specified to the JDBC driver using the java.sql.Statement.setQueryTimeout() method.

The method sets the number of seconds the driver will wait for a Statement object to execute. 

If your JDBC driver does not support this method, it may throw an exception and the timeout value is ignored

Once the JDBC statement times out, the Oracle JDBC driver throws a java.sql.SQLException: ORA-01013: user requested cancel of current operation to the server log.

Statement Timeout = 600s (Datasource : {Name})
