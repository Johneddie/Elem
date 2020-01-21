https://memlisapd01.mem.int/ServiciosDGFM/WSUtilitarioDGFM.svc?WSDL

[root@p005sps01 bin]# ./wsadmin.sh -host p005sps01 -port 8880 -conntype SOAP -user wasadmin -password xxxxxx -lang jython
WASX7209I: Connected to process "PS_PRD01.AppCluster.p005sps01Node01.0" on node p005sps01Node01 using SOAP connector;  The type of process is: ManagedProcess
WASX7031I: For help, enter: "print Help.help()"
wsadmin>AdminTask.BPMInstallOfflinePackage('[-inputFile /root/1.1.17-PS_PROD_OFFLINE.zip]')
WASX7015E: Exception running command: "AdminTask.BPMInstallOfflinePackage('[-inputFile /root/1.1.17-PS_PROD_OFFLINE.zip]')"; exception information:
java.lang.Exception: java.lang.Exception: PreparedStatementCallback; SQL [insert into LSW_ENV_VAR_DEFAULT (ENV_VAR_DEFAULT_ID,VERSION_ID,VALUE,GUID,LAST_MODIFIED,ENV_TYPE_ID,ENV_VAR_ID,LAST_MODIFIED_BY_USER_ID) values (?,?,?,?,?,?,?,?)]; ORA-01400: cannot insert NULL into ("PSUSER"."LSW_ENV_VAR_DEFAULT"."VALUE")
; nested exception is java.sql.SQLIntegrityConstraintViolationException: ORA-01400: cannot insert NULL into ("PSUSER"."LSW_ENV_VAR_DEFAULT"."VALUE")

