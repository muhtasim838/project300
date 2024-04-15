<!DOCTYPE html>
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  
  
  <title>TTTP2543</title>
  <meta name="generator" content="Bootply">
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <!-- <link rel="icon" type="image/ico" href="https://lrgs.ftsm.ukm.my/users/a123456/tutorial1/favicon.ico"> -->
  <link href="./tutorial1_files/bootstrap.min.css" rel="stylesheet">
	<!--[if lt IE 9]>
		<script src="//html5shim.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->
    <link href="./tutorial1_files/styles.css" rel="stylesheet">
    <script type="text/javascript" src="./tutorial1_files/shCore.js.download"></script>
    <script type="text/javascript" src="./tutorial1_files/shBrushXml.js.download"></script>
    <link type="text/css" rel="stylesheet" href="./tutorial1_files/shCoreDefault.css">
    <script type="text/javascript">SyntaxHighlighter.all();</script>
  </head>
  <body data-new-gr-c-s-check-loaded="14.1084.0" data-gr-ext-installed="" style="">
    <nav class="navbar navbar-default navbar-fixed-top" role="banner">
      <div class="container">
        <div class="navbar-header">
          <a href="https://metrouni.edu.bd/" class="navbar-brand">Metropolitan University, Department of Computer Science & Engineering</a>
        </div>
      </div>
    </nav>

    <div id="masthead">
      <div class="container">
        <div class="row">
          <div class="col-md-10">
            <h1>Project 300
              <p class="lead"></p>
              <p class="lead">Portable XAMPP and Sublime Editor Setup</p>
              
              </h1><h5><em>by Dewan Ahmed Muhtasim, lecturer, CSE</em></h5>
            
          </div>
          <div class="col-md-2">
            <div class="row">
              <div class="col-sm-12" align="right"><br><br>
                <img src="./tutorial1_files/MU.jpg" class="img-responsive">
              </div>
            </div>
          </div>
        </div>
      </div><!--/container-->
    </div><!--/masthead-->


    <!--main-->
    <div class="container">
     <div class="row">
      <!--left-->
      <div class="col-md-3" id="leftCol">
        <ul class="nav nav-stacked affix" id="sidebar">
          <li class=""><a href="">1. Install XAMPP</a></li>
          <li class=""><a href="">2. Stop Local Services</a></li>
          <li class=""><a href="">3. Start Apache Web Server</a></li>
          <li class=""><a href="">4. Test Localhost</a></li>
          <li class=""><a href="">5. Start MySQL Database Server</a></li>
          <li class=""><a href="">6. Open phpMyAdmin</a></li>
          <li class=""><a href="">7. Install Sublime Text Editor</a></li>       
        </ul>
      </div><!--/left-->

      <!--right-->
      <div class="col-md-9">
        <h2 id="xampp">1. Install XAMPP</h2>
        <p>
          In this course, we need to developed web pages. Later, in the second half of the semester, you are going to develop a web-based system. If the pages are static HTML and CSS files, the software requirement is simple, where you only need a text editor (like Notepad or Sublime text editor) and a web browser to view the pages. However, you need more than that because besides those files, you are going to develop server side scripts in PHP. The PHP will do many operations that include connecting to a database. To run the PHP, you need a web server. On the other hand, to have a database, surely you need a database server. To make things easier, lets use a software package called XAMPP that can help you to install both the web and database server with minimum effort to configure settings and so on.
        </p>
        <p>
          XAMPP is a free and open source cross-platform web server solution stack package developed by Apache Friends, consisting mainly of the Apache HTTP Server, MySQL database, and interpreters for scripts written in the PHP and Perl programming languages. XAMPP is a portable software. So it can be run without installation to system folder and it does not leave any traces in system registry. It means you can install a web server and a database server into a portable disk and start the services once you needed.
        </p>
        <p>
          Firstly, you need to prepare a flash drive or an external hard drive. Make sure that you have minimum of <kbd>1GB</kbd> of free spaces in the drive. In this tutorial, I assume that you have a flash drive. Then, go to this address:
          </p><pre>https://www.apachefriends.org/download.html</pre>
        <p></p>
        <p>
          In there, you’ll see various kinds of packages. Please:
        </p>
        <ol>
          <li>Click <kbd>More Downloads</kbd></li>
          <li>Click <kbd>XAMPP Windows</kbd></li>
          <li>Click the latest version, let say <kbd>8.2.12 / PHP 8.2.12	</kbd></li>
          <li>Click the portable version of xampp like <kbd>xampp-windows-x64-8.2.12-0-VS16-installer</kbd> to install it</li>
        </ol>
        <p>
          Once the downloading has completed, double click the installer file to start the XAMPP setup process. Press <kbd>Next &gt;</kbd> until you see a windows as below:
        </p>
        <p>
          <img src="./tutorial1_files/1-1.png" class="img-responsive">
        </p>
        <p>
          For this class, we only need the followings:
          </p><ul>
            <li>Apache, by default it is selected</li>
            <li>MySQL</li>
            <li>PHP, by default it is selected</li>
            <li>phpMyAdmin</li>
          </ul>
          For project 300, you need to select the above items. Press <kbd>Next &gt;</kbd> to proceed.
        <p></p>
        <p>
          In the next window, as below, change the installation folder to your flash drive. In my case, my flash drive is in Drive <kbd>C:\XAMPP</kbd>. Your flash drive may had been assigned to another drive letter. Change the drive letter and maintain the <kbd>xampp</kbd> folder. Then, press <kbd>Next &gt;</kbd>.
        </p>
        <p>
          <img src="./tutorial1_files/1-2.png" class="img-responsive">
        </p>
        <p>
          Press the <kbd>Next &gt;</kbd> buttons until the installation starts as below:
        </p>
        <p>
          <img src="./tutorial1_files/1-3.png" class="img-responsive">
        </p>
        <p>
          It will take some time to complete. Once the installation is completed, you will see a window like this:
        </p>
        <p>
          <img src="./tutorial1_files/1-4.png" class="img-responsive">
        </p>
        <p>
          Uncheck the checkbox so that you will not start the Control Panel now. Press <kbd>Finish</kbd> to end the installation.
        </p>
        <hr>

        <h2 id="stop">2. Stop Local Services that Interrupt Web and Database Services</h2>
        <p>
          In this section, you will test whether or not your local computer has services that will interfere the Apache web server and MySQL database server. Apache web server runs, by default, in port 80 while MySQL database server runs in port 3306. So, you need to make sure that no other software in your local computer use those port numbers. Other software that might use the port 80 are Internet Information Server (IIS) and Skype.
        </p>
        <p>
          Firstly, you need to scan all opened (used) ports in your local computer. To do that, run your <kbd>Command Prompt</kbd>.
        </p>
        <p class="bg-success">
          <button class="btn btn-success btn-xs" type="submit">Updated: 15/04/2024</button> Make sure that you run it as <kbd>Run as administrator</kbd>.
        </p>
        <p>
          Type the following command and press <kbd>Enter</kbd>.
          </p><pre>netstat -a -n -o</pre>
          In my case, I will see outputs like this:
        <p></p>
        <p>
          <img src="./tutorial1_files/2-1.png" class="img-responsive">
        </p>
        <p>
          As you can see in above image, in my case, both 80 and 3306 ports of my computer are not in used by any unknown software. Please refer to the <kbd>Local Address</kbd> column. Port number is a number after the IP address. The address format is <kbd>x.x.x.x:port</kbd>. In your case, your computer might show different numbers. If you can't find port 80 and 3306 under the <kbd>Local Address</kbd>, it means you are OK. You no need to kill any proceses. You can proceed to Part 3.
        </p>
        <p>
          For example, let's say my port 80 is used by a software identified by PID = 5804. To kill the process, execute this command:
          </p><pre>taskkill /pid 5804</pre>
          Replace the 5804 with a number showed in your console. The output of this operation is:
        <p></p>
        <p>
          <img src="./tutorial1_files/2-2.png" class="img-responsive">
        </p>
        <p>
          For example, let's say my port 3306 is used by a software identified by PID = 6540. I would kill the process, by executing this command:
          </p><pre>taskkill /pid 6540 /f</pre>
          <kbd>/f</kbd> is to force the process to stop. My console looks like this:
        <p></p>
        <p>
          <img src="./tutorial1_files/2-3.png" class="img-responsive">
        </p>
        <p>
          Close your <kbd>Command Prompt</kbd> console to end this part.
        </p>

        <hr>

        <h2 id="apache">3. Start Apache Web Server</h2>
        <p>
          To start your web server, you need to open the XAMPP Control Panel. Open your file explorer and browse your flash drive until the installation <kbd>drive:\xampp\</kbd> folder.
        </p>
        <p class="bg-success">
          <button class="btn btn-success btn-xs" type="submit">Updated: 15/04/2024</button> Since you will use your flash drive in different computers, it good to make a habit to setup the XAMPP first. This is to ensure that your XAMPP can properly run with correct configuration. For example, different computers will assign your flash drive with a different drive letter. You can do this by double clicking the <kbd>setup_xampp.bat</kbd> file. You will see output like this:
        </p>
        <p>
          <img src="./tutorial1_files/3-4.png" class="img-responsive">
        </p>
        <p>
          Type <kbd>1</kbd> and press <kbd>Enter</kbd>. You will get:
        </p>
        <p>
          <img src="./tutorial1_files/3-5.png" class="img-responsive">
        </p>
        <p>
          On the other hand, if you get <kbd>Nothing to do</kbd> message like in the image below, it means you are all set. The current configuration is matched with your current flash drive. Just press any key to close the command prompt dialog.
        </p>
        <p>
          <img src="./tutorial1_files/3-6.png" class="img-responsive">
        </p>
        <p>
          Once OK then, double click the <kbd>xampp-control.exe</kbd> file.
        </p>
        <p>
          <img src="./tutorial1_files/3-1.png" class="img-responsive">
        </p>
        <p>
          You will see a Control Panel window like this:
        </p>
        <p>
          <img src="./tutorial1_files/3-2.png" class="img-responsive">
        </p>
        <p>
          To start the Apache web server, click the <kbd>Start</kbd> button of the Apache module. Wait until you will see the Apache module is highlighted as <kbd>green</kbd>. This means the service is started as below.
        </p>
        <p>
          <img src="./tutorial1_files/3-3.png" class="img-responsive">
        </p>
        <div class="panel panel-primary">
          <div class="panel-heading">Try-it-yourself</div>
          <div class="panel-body">
            Try stop the service and start it back.
          </div>
        </div>
        <hr>

        <h2 id="localhost">4. Test localhost</h2>
        <p>
          Once the web service is started, you can test to open web pages from your localhost (your local computer). To open a default page of XAMPP, open your <kbd>Web Browser</kbd> and type this URL:
          </p><pre>http://localhost</pre>
          You will be directed to <kbd>localhost/dashboard/</kbd> like this page:
        <p></p>
        <p>
          <img src="./tutorial1_files/4-1.png" class="img-responsive">
        </p>
        <p>
         Having this page means that your web server is up and running. All web pages that you want to host must be saved in <kbd>drive:\xampp\htdocs</kbd> folder. The <kbd>dashboard</kbd> in the URL is actually a folder in the <kbd>htdocs</kbd> folder. Open your file explorer and browse up to the <kbd>dashboard</kbd> folder.
       </p>

       <div class="panel panel-primary">
        <div class="panel-heading">Try-it-yourself</div>
        <div class="panel-body">
          Observe the <kbd>dashboard</kbd> folder and it contents. Explore other folders in <kbd>htdocs</kbd>.
        </div>
      </div>

      <hr>

      <h2 id="mysql">5. Start MySQL Database Server</h2>
      <p>
        Open back the XAMPP Control Panel. To start the MySQL database server, click the <kbd>Start</kbd> button of the MySQL module. Wait until you will see the MySQL module is highlighted as <kbd>green</kbd> as below.
      </p>
      <p>
        <img src="./tutorial1_files/5-1.png" class="img-responsive">
      </p>

      <hr>

      <h2 id="phpmyadmin">6. Open phpMyAdmin</h2>
      <p>
        phpMyAdmin is a free and open source tool written in PHP intended to handle the administration of MySQL with the use of a web browser. It can perform various tasks such as creating, modifying or deleting databases, tables, fields or rows; executing SQL statements; or managing users and permissions.
      </p>
      <p>
        To start phpMyAdmin, open your web browser and enter this URL:
        </p><pre>http://localhost/phpmyadmin/</pre>
        You will open a page like this:
      <p></p>
      <p>
        <img src="./tutorial1_files/6-1.png" class="img-responsive">
      </p>
      <hr>
      <div class="panel panel-primary">
        <div class="panel-heading">Try-it-yourself</div>
        <div class="panel-body">
          Try create a database with few tables. Insert few data in the tables.
        </div>
      </div>
      <div class="panel panel-warning">
        <div class="panel-heading">Web Resources</div>
        <div class="panel-body">
          Tutorials on phpMyAdmin: <a class="btn btn-warning btn-xs" href="https://www.siteground.com/tutorials/phpmyadmin/" role="button">https://www.siteground.com/tutorials/phpmyadmin/</a><br>
          Videos on phpMyAdmin: <a class="btn btn-warning btn-xs" href="https://www.youtube.com/watch?v=co-xyHRdHRg" role="button">https://www.youtube.com/watch?v=co-xyHRdHRg</a>
        </div>
      </div>

      <hr>

      <h2 id="sublime">7. Install Sublime Text Editor</h2>
      <p>
        In this project, we will write our codes in a text editor. Obviously, if you are using Windows operating system, the Notepad will do the job. But, we need a better text editor. There are may good text editors like the Adobe Dreamweaver CS4 HTML editor, Atom, Brackets and Notepad++. Instead of those editors we are going to use the Sublime Text Editor. Please note, you can use any editor you like. Sublime is a sophisticated text editor for code, markup and prose. It has a slick user interface, extraordinary features and amazing performance. The most important is that it is <kbd>FREE</kbd>. Most of expert users like to use text editor to compose HTML and PHP to gain flexibilty and performance. To download a Sublime Editor, go to this URL:
        </p><pre>https://www.sublimetext.com/download</pre>
      <p></p>
      <p>
        In there, you’ll see various kinds of versions. Click on <kbd>windows</kbd> to download the setupfile.
      </p>
      <p>
        Once the downloading has completed, double click the installer file to start the Sublime setup process. Press <kbd>Next &gt;</kbd> until you see a windows as below:
      </p>
      <p>
        <img src="./tutorial1_files/7-1.png" class="img-responsive">
      </p>
      <p>
        Change the installation folder to your flash drive. In my case, my flash drive is in Drive <kbd>C:\</kbd>. Maintain the <kbd>Sublime Text 4</kbd> as the name of the installation folder. Then, press <kbd>Next &gt;</kbd> until you press <kbd>Install</kbd>. To end the installation process, press <kbd>Finish</kbd> button in the last installation window as below:
      </p>
      <p>
        <img src="./tutorial1_files/7-2.png" class="img-responsive">
      </p>
      <p>
        Open your file explorer and browse, or search for <kbd>Sublime Text</kbd> folder.Double click the <kbd>sublime_text.exe</kbd> file and you will see a text editor like this:
      </p>
      <p>
        <img src="./tutorial1_files/7-3.png" class="img-responsive">
      </p>
      <p>
        In this way, you make Sublime Text Editor as a portable software. You will carry this text editor in your flash drive anywhere anytime. Once you start your web and database servers, you can open Sublime and start coding.
      </p>
      <p>
        As a start, lets create your first HTML page using Sublime and save in <kbd>htdocs</kbd> folder. Create a new file. First thing is to set the type and syntax of your file by selecting <kbd>HTML</kbd> at the bottom-right corner of your Sublime like:
      </p>
      <p>
        <img src="./tutorial1_files/8-7.png" class="img-responsive">
      </p>
      <p>
         Later if you are composing a PHP file, then you need to select <kbd>PHP</kbd> in the list. Next, save the file as <kbd>hello.html</kbd>. Copy and paste the following codes in Sublime. Alternatively, you can type <kbd>html</kbd> and press <kbd>tab</kbd>. A skeleton of HTML code will be automatically created.
      </p>
      <div><div id="highlighter_563853" class="syntaxhighlighter  html"><div class="toolbar"><span><a href="https://lrgs.ftsm.ukm.my/users/a123456/tutorial1/tutorial1.html#" class="toolbar_item command_help help">?</a></span></div><table border="0" cellpadding="0" cellspacing="0"><tbody><tr><td class="gutter"><div class="line number1 index0 alt2">1</div><div class="line number2 index1 alt1">2</div><div class="line number3 index2 alt2">3</div><div class="line number4 index3 alt1">4</div><div class="line number5 index4 alt2">5</div><div class="line number6 index5 alt1">6</div><div class="line number7 index6 alt2">7</div><div class="line number8 index7 alt1">8</div><div class="line number9 index8 alt2">9</div><div class="line number10 index9 alt1">10</div></td><td class="code"><div class="container"><div class="line number1 index0 alt2"><code class="html plain">&lt;!DOCTYPE html&gt;</code></div><div class="line number2 index1 alt1"><code class="html plain">&lt;</code><code class="html keyword">html</code><code class="html plain">&gt;</code></div><div class="line number3 index2 alt2"><code class="html plain">&lt;</code><code class="html keyword">head</code><code class="html plain">&gt;</code></div><div class="line number4 index3 alt1"><code class="html plain">&lt;</code><code class="html keyword">meta</code> <code class="html color1">charset</code> <code class="html plain">= </code><code class="html string">"utf-8"</code><code class="html plain">&gt;</code></div><div class="line number5 index4 alt2"><code class="html plain">&lt;</code><code class="html keyword">title</code><code class="html plain">&gt;Hello&lt;/</code><code class="html keyword">title</code><code class="html plain">&gt;</code></div><div class="line number6 index5 alt1"><code class="html plain">&lt;/</code><code class="html keyword">head</code><code class="html plain">&gt;</code></div><div class="line number7 index6 alt2"><code class="html plain">&lt;</code><code class="html keyword">body</code><code class="html plain">&gt;</code></div><div class="line number8 index7 alt1"><code class="html plain">&lt;</code><code class="html keyword">p</code><code class="html plain">&gt;Now you know how to start your Project 300!&lt;/</code><code class="html keyword">p</code><code class="html plain">&gt;</code></div><div class="line number9 index8 alt2"><code class="html plain">&lt;/</code><code class="html keyword">body</code><code class="html plain">&gt;</code></div><div class="line number10 index9 alt1"><code class="html plain">&lt;/</code><code class="html keyword">html</code><code class="html plain">&gt;</code></div></div></td></tr></tbody></table></div></div>
      <p>
        <img src="./tutorial1_files/7-4.png" class="img-responsive">
      </p>
      <p>
        Save the HTML file in your XAMPP\htdocs folder by clicking save as. Open your web browser and type this URL:
        </p><pre>http://localhost/hello.html</pre>
        You will get a page like this:
      <p></p>
      <p>
        <img src="./tutorial1_files/7-5.png" class="img-responsive">
      </p>

      <hr>

      <div class="panel panel-primary">
        <div class="panel-heading">Try-it-yourself</div>
        <div class="panel-body">
          Explore all the menus and functionalities of Sublime Text Editor. Please try the below tips and tricks. You will find that Sublime is very awesome. If you have experience working with other editors, go with them.
        </div>
      </div>
      <div class="panel panel-warning">
        <div class="panel-heading">Web Resources</div>
        <div class="panel-body">
          Tip and tricks of Sublime: <a class="btn btn-warning btn-xs" href="https://generalassemb.ly/blog/sublime-text-3-tips-tricks-shortcuts/" role="button">https://generalassemb.ly/blog/sublime-text-3-tips-tricks-shortcuts/</a><br>
          Videos on Sublime: <a class="btn btn-warning btn-xs" href="http://code.tutsplus.com/courses/perfect-workflow-in-sublime-text-2" role="button">http://code.tutsplus.com/courses/perfect-workflow-in-sublime-text-2</a>
        </div>
      </div>

    </div><!--/right-->
  </div><!--/row-->
</div><!--/container-->



<!-- script references -->
<script src="./tutorial1_files/jquery.min.js.download"></script>
<script src="./tutorial1_files/bootstrap.min.js.download"></script>
<script src="./tutorial1_files/scripts.js.download"></script>

</body><grammarly-desktop-integration data-grammarly-shadow-root="true"></grammarly-desktop-integration></html>
