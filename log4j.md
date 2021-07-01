<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
</head>
<body>
<h3>A short summary on the use of the logging service. How to use it in practice.</h3>
<h2>Start</h2>
<p>
  In each class where you want to use the logger, create an instance of it, e.g.</p>
<i>
  private static Logger logger = LogManager.getLogger(BuildingController.class);
</i>

<h4>the name of the specific class must be in brackets</h4>

<p>
  Logger and LogManager should be automatically imported. To be sure, check that they are from the
  apache.logging.log4j class.
</p>

<h2>Imports</h2>
<p>
  The imports should be from:
</p>
<i>org.apache.logging.log4j.LogManager
</i>
<p>and</p>
<i>
  org.apache.logging.log4j.Logger.
</i>


<h2>Logging</h2>
<p>
  Then you can use the logger, using the following style:
</p>

<p>
  logger."log type setting"(and here the logging itself...), e.g.:
</p>

<i>
  logger.info("POST /buildings " + HttpStatus.OK + " " + createdBuilding);
  or
  logger.error("HttpStatus: 400 " + e.getMessage());
</i>
<p>
  variables, strings, getters, etc. can be used in the log entry

Then the write is made to the logs.log file.
  Name and folder we can change.
</p>
<h3>
    Custom Log Levels
</h3>
<p> 
The built-in log levels for log4j2 are:

OFF, 
FATAL, 
ERROR, 
WARN, 
INFO, 
DEBUG, 
TRACE, 
ALL
</p>

<h3>Environment variables</h3>
<p>in environment variables I set the value of the entry from info above. of course we can discuss
  and change what will be suitable for our project</p>
</body>
</html>
