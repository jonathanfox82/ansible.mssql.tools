Role Name
=========

MSSQL tools for Linux based on https://docs.microsoft.com/en-us/sql/linux/sql-server-linux-setup-tools
Useful when you just want to have the ability to run SQL queries in Ansible shell commands against MSSQL databases without installing a full role of SQL Server.

Usage of sqlcmd below

sqlcmd   
   -a packet_size  
   -A (dedicated administrator connection)  
   -b (terminate batch job if there is an error)  
   -c batch_terminator  
   -C (trust the server certificate)  
   -d db_name  
   -e (echo input)  
   -E (use trusted connection)  
   -f codepage | i:codepage[,o:codepage] | o:codepage[,i:codepage] 
   -g (enable column encryption) 
   -G (use Azure Active Directory for authentication)
   -h rows_per_header  
   -H workstation_name  
   -i input_file  
   -I (enable quoted identifiers)  
   -j (Print raw error messages)
   -k[1 | 2] (remove or replace control characters)  
   -K application_intent  
   -l login_timeout  
   -L[c] (list servers, optional clean output)  
   -m error_level  
   -M multisubnet_failover  
   -N (encrypt connection)  
   -o output_file  
   -p[1] (print statistics, optional colon format)  
   -P password  
   -q "cmdline query"  
   -Q "cmdline query" (and exit)  
   -r[0 | 1] (msgs to stderr)  
   -R (use client regional settings)  
   -s col_separator  
   -S [protocol:]server[instance_name][,port]  
   -t query_timeout  
   -u (unicode output file)  
   -U login_id  
   -v var = "value"  
   -V error_severity_level  
   -w column_width  
   -W (remove trailing spaces)  
   -x (disable variable substitution)  
   -X[1] (disable commands, startup script, environment variables, optional exit)  
   -y variable_length_type_display_width  
   -Y fixed_length_type_display_width  
   -z new_password   
   -Z new_password (and exit)  
   -? (usage)  


Requirements
------------

None

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: jonathanfox82.mssql-tools }

License
-------

BSD

