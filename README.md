solr.init.d - A SUSE Linux init script for starting Apache Solr
===============================================================

This is a SUSE Linux init script for running [Apache Solr](http://lucene.apache.org/solr/). It was based off of the skeleton script that is provided with SUSE Linux Enterprise.

The script utilizes the [Daemon](http://libslack.org/daemon/) utility.

There are a few variables that will need to be modified for your environment. Look for the variables DAEMON, SOLR_DIR, SOLR_LOG, and SOLR_USER in the script and modify them if necessary.

Installing the script
---------------------
After copying the file to /etc/init.d/solr the service can be installed with the following command:

	# insserv solr

Once installed the service can be started, stopped, restarted, etc... like this:

	# service solr start
	# service solr status
	# service solr restart
	# service solr stop
