<html xmlns="http://www.w3.org/1999/xhtml">
<head>
    <title>Log File Monitor</title>
    <meta http-equiv="Content-Type" content="text/html; charset=UTF-8"/>
    <meta http-equiv="X-UA-Compatible" content="IE=EmulateIE8" />
    <meta content="Scroll Wiki Publisher" name="generator"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/liquid.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/blueprint/print.css" media="print"/>
    <link type="text/css" rel="stylesheet" href="css/content-style.css" media="screen, projection, print"/>
    <link type="text/css" rel="stylesheet" href="css/screen.css" media="screen, projection"/>
    <link type="text/css" rel="stylesheet" href="css/print.css" media="print"/>
</head>
<body>
                <h1>Log File Monitor</h1>
    <div class="section-2"  id="114557276_LogFileMonitor-Overview"  >
        <h2>Overview</h2>
    <p>
    </p>
    <div class="confbox admonition admonition-info">
    <p>
Previously called &quot;Windows Log File Monitor&quot; but updated to now support both Windows and Linux    </p>
    </div>
    <p>
The monitor searches a windows or Linux log file for text or regex expression and returns if a new line was found, and the last line number to contain the regex.    </p>
    <p>
It stores the last result and position in the monitored file in a SQL database so that it knows where it ended the last time it ran so it's not reading the same lines over and over. If the log file rolls over the monitor is smart enough to see that and starts from the beginning of the file again. The table in the database can be created by running the attached script or you can use the screenshot from the Design view in the table to manually enter the values. The script will create the table on a database called dynaTracePluginDB. Change this name if you desire.    </p>
    <p>
    </p>
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/114557276/LogRecords_Schema_Screenshot.jpg" alt="images_community/download/attachments/114557276/LogRecords_Schema_Screenshot.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/114557276/LogFileMonitor_Schema_Screenshot.jpg" alt="images_community/download/attachments/114557276/LogFileMonitor_Schema_Screenshot.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/114557276/log_file_scrapper2.jpg" alt="images_community/download/attachments/114557276/log_file_scrapper2.jpg" class="" />
            </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
LogRecord Table Schema    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
LogFileMonitor Schema    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Monitor Properties    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/114557276/log_file_scrapper.jpg" alt="images_community/download/attachments/114557276/log_file_scrapper.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
            <img src="images_community/download/attachments/114557276/log_file_scrapper_measures.jpg" alt="images_community/download/attachments/114557276/log_file_scrapper_measures.jpg" class="" />
            </p>
            </td>
                <td rowspan="1" colspan="1">
                </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Monitor Properties    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Log File Monitor Measures    </p>
            </td>
                <td rowspan="1" colspan="1">
                </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    
    <div class="section-2"  id="114557276_LogFileMonitor-PluginDetails"  >
        <h2>Plugin Details</h2>
    
    <div class="tablewrap">
        <table>
<thead class=" "></thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Plug-In Versions    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_149553403_1_com.logfile_3.14.15.jar">Log File Monitor for Windows and Linux</a> (compatible with dynaTrace 4.2+)<br/><a href="attachments_114688050_1_com.log.scrapper_3.14.15.jar">Windows Log File Monitor 3.14.15</a> (compatible with dynaTrace 4.2+)<br/><a href="attachments_149553409_1_LogFileMonitor.sql">SQL Command to create LogFileMonitor Table</a><br/><a href="attachments_149553411_1_LogRecords.sql">SQL Commands to create LogRecords Table</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Author    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Derek Abing    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
License    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="attachments_5275722_2_dynaTraceBSD.txt">dynaTrace BSD</a>    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Support    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
<a href="https://community/display/DL/Support+Levels#SupportLevels-Community">Not Supported </a><br/>If you have any questions or suggestions for these plugins, please add a comment to this page, use our <a href="https://community.dynatrace.com/community/pages/viewpage.action?pageId=46628918">forum</a>, or drop us an email at <a href="mailto:apmcommunity@compuware.com">apmcommunity@compuware.com</a>!    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Known Problems    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Release History    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
2013-03-12 Initial Release for Windows Log Files Only    </p>
    <p>
2013-12-18 Log File Monitor for Windows and Linux    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="114557276_LogFileMonitor-ProvidedMeasures"  >
        <h2>Provided Measures</h2>
    <p>
<strong class=" ">Line Number</strong>: The Line Number of the last known occurance of the specified search term.<br/><strong class=" ">New Message</strong>: Returns a 1 if a new entry was made to log file with the search term specified.<br/><strong class=" ">Number of Messages</strong>: The number of lines that matched the Search Term.    </p>
    </div>
    <div class="section-2"  id="114557276_LogFileMonitor-Configuration"  >
        <h2>Configuration</h2>
    <div class="tablewrap">
        <table>
<thead class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
Name    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Value    </p>
            </td>
        </tr>
</thead><tfoot class=" "></tfoot><tbody class=" ">    <tr>
            <td rowspan="1" colspan="1">
        <p>
OS    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Dropdown for selecting either Windows or Linux    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Directory    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The directory on the server that contains the log file.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
File Regex    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
If this is selected then the file must be specified in terms of a regex expression. If the directory contains multiple files that match the regex the newest file will be selected    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
File    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The File that you wish to search. If the File Regex option is checked, then this must be a regex.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Search Term    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
A regex of what you wish to search for within the log file    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
SQL Server    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
SQL Server to contain the repository of log file searches    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
SQL Port    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Port to connect to on the SQL Server    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Database    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The database to use for the log file repository.    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
SQL Username    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Username used to connect to the SQL Database    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
SQL Password    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
The password for the username used to connect to the SQL database    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Additional Lines    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
Amount of additional lines to include in file after the log message is found    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Skip Additional Records    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
If this box is checked, records included in the additional lines will be skipped for processing    </p>
            </td>
        </tr>
    <tr>
            <td rowspan="1" colspan="1">
        <p>
Keep Historical Record    </p>
            </td>
                <td rowspan="1" colspan="1">
        <p>
If this box is checked, a historical record of each log message will be added to the LogRecords database.  This database can then be queried for a list of all log messages matching a specific search and the corresponding timestamps    </p>
            </td>
        </tr>
</tbody>        </table>
            </div>
    </div>
    <div class="section-2"  id="114557276_LogFileMonitor-Installation"  >
        <h2>Installation</h2>
    <p>
Import the Plugin into the dynaTrace Server. For details how to do this please refer to the <a href="https://community/display/DOCDT50/Manage+and+Develop+User+Plugins">dynaTrace documentation</a>.    </p>
    </div>
            </div>
        </div>
        <div class="footer">
        </div>
    </div>
</body>
</html>
