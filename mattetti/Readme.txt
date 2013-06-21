Usage:
Add in user.properties:
jmeter.save.saveservice.output_format=csv
jmeter.save.saveservice.data_type=false
jmeter.save.saveservice.label=true
jmeter.save.saveservice.response_code=true
jmeter.save.saveservice.response_data.on_error=false
jmeter.save.saveservice.response_message=false
jmeter.save.saveservice.successful=true
jmeter.save.saveservice.thread_name=true
jmeter.save.saveservice.time=true
jmeter.save.saveservice.subresults=false
jmeter.save.saveservice.assertions=false
jmeter.save.saveservice.latency=true
jmeter.save.saveservice.bytes=true
jmeter.save.saveservice.hostname=true
jmeter.save.saveservice.thread_counts=true
jmeter.save.saveservice.sample_count=true
jmeter.save.saveservice.response_message=false
jmeter.save.saveservice.assertion_results_failure_message=false
jmeter.save.saveservice.timestamp_format=HH:mm:ss
jmeter.save.saveservice.default_delimiter=;
jmeter.save.saveservice.print_field_names=true

summariser.name=summary
# interval between summaries (in seconds) default 3 minutes
summariser.interval=10
# Write messages to log file
summariser.log=true
# Write messages to System.out
summariser.out=true

Use nightly build:
http://jmeter.apache.org/nightly.html
Download the _bin and _lib files
Unpack the archives into the same directory structure
The other archives are not needed to run JMeter. 

Load Test in NON GUI Mode
<JMETER_HOME>/bin/jmeter -t <Path to Test Plan> -n -l <path to results>/results.csv


If you want beautiful graphs, see JP@GC but only use them after the load test is finished, you can generate the graphs
