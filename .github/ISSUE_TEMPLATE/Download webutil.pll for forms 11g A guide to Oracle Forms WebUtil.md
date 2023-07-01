# How to Download and Use Webutil.pll for Oracle Forms 11g
 
Webutil.pll is a library that provides a set of PL/SQL functions and procedures that enable Oracle Forms developers to access client-side resources and functionalities when deploying their applications over the web. Webutil.pll is included with all Oracle Forms 11g and newer installations, but it may require a third party library called JACOB (Java COM Bridge) to work properly. In this article, we will show you how to download and use webutil.pll for Oracle Forms 11g.
 
**Download > [https://t.co/rYxBIKcaZ5](https://t.co/rYxBIKcaZ5)**


 
## Step 1: Download webutil.pll
 
You can download webutil.pll from the Oracle website[^2^] or from your Oracle Forms installation directory. The default location of webutil.pll is `$ORACLE_HOME/forms/webutil/webutil.pll`, where `$ORACLE_HOME` is the path of your Oracle Forms installation. You can also find webutil.pll in the `$ORACLE_HOME/forms/user_manuals/webutil` directory, along with other documentation and examples.
 
## Step 2: Attach webutil.pll to your form
 
To use webutil.pll in your form, you need to attach it as a library. To do this, open your form in Oracle Forms Builder and go to `Navigator -> Attached Libraries`. Click on the `+` icon to create a new attached library and browse to the location of webutil.pll. Select it and click `OK`. You should see webutil.pll listed under the attached libraries section.
 
## Step 3: Configure webutil parameters
 
To configure webutil parameters, you need to open the `WebUtil Utility` tab in your form. This tab is available in Oracle Forms 11g release 1 and release 2, but not in release 0. To access this tab, go to `Navigator -> Form -> WebUtil Utility`. Here you can specify the path of the webutil.pll file and the URL used for uploading files when working with attached data sources. You can also choose a language for the webutil messages from a list of supported languages.
 
## Step 4: Call webutil functions and procedures
 
Once you have attached and configured webutil.pll, you can call its functions and procedures from your PL/SQL code. Webutil provides a number of functions and procedures that mimic the native Forms built-ins, such as `Client_Host`, `Client_Text_IO`, `WebUtil_File.File_Open_Dialog`, etc. You can also use webutil to access client-side features such as OLE, clipboard, printer, etc. For a complete list of webutil functions and procedures, refer to the webutil documentation[^2^].
 
How to install Oracle WebUtil for Forms 11g,  WebUtil.pll compile error on Forms 11g,  A simplified guide to understanding WebUtil,  Forms 11g Client\_Host command using WebUtil,  WebUtil configuration steps for Forms 11g,  How to access local resources with WebUtil,  WebUtil and JACOB library for Forms 11g,  WebUtil and Pluggable Java Component for Forms 11g,  How to use WebUtil\_File\_Transfer in Forms 11g,  How to enable debugging for WebUtil in Forms 11g,  How to use WebUtil\_Clipboard in Forms 11g,  How to use WebUtil\_OLE in Forms 11g,  How to use WebUtil\_DB in Forms 11g,  How to use WebUtil\_Java\_Import in Forms 11g,  How to use WebUtil\_ClientInfo in Forms 11g,  How to use WebUtil\_Browser in Forms 11g,  How to use WebUtil\_MessageBox in Forms 11g,  How to use WebUtil\_IniFile in Forms 11g,  How to use WebUtil\_Registry in Forms 11g,  How to use WebUtil\_Printer in Forms 11g,  How to use WebUtil\_DDE in Forms 11g,  How to use WebUtil\_Mail in Forms 11g,  How to use WebUtil\_Sound in Forms 11g,  How to use WebUtil\_CAPI in Forms 11g,  How to use WebUtil\_Win\_API in Forms 11g,  How to use WebUtil\_ShellExecute in Forms 11g,  How to use WebUtil\_Host\_Blocking in Forms 11g,  How to use WebUtil\_Host\_NonBlocking in Forms 11g,  How to use WebUtil\_Host\_With\_Callback in Forms 11g,  How to use WebUtil\_Host\_With\_Return\_Value in Forms 11g,  How to use WebUtil\_Host\_With\_Return\_String\_Array in Forms 11g,  How to use WebUtil\_Host\_With\_Return\_Binary\_Array in Forms 11g,  How to use WebUtil\_File\_Open\_Dialog in Forms 11g,  How to use WebUtil\_File\_Save\_Dialog in Forms 11g,  How to use WebUtil\_File\_Delete\_File\_On\_Client in Forms 11g,  How to use WebUtil\_File\_Rename\_File\_On\_Client in Forms 11g,  How to use WebUtil\_File\_Copy\_File\_On\_Client\_To\_Server in Forms 11g,  How to use WebUtil\_File\_Copy\_File\_On\_Server\_To\_Client in Forms 11g,  How to use WebUtil\_File\_Copy\_File\_On\_Server\_To\_Server in Forms 11g,  How to use WebUtil\_File\_Copy\_File\_On\_Client\_To\_Client in Forms 11g,  How to use WebUtil\_File\_Get\_Name\_From\_Path\_On\_Client in Forms 11g,  How to use WebUtil\_File\_Get\_Name\_From\_Path\_On\_Server in Forms 11g,  How to use WebUtil\_File\_Get\_Path\_From\_Name\_On\_Client in Forms 11g,  How to use WebUtil\_File\_Get\_Path\_From\_Name\_On\_Server in Forms 11g,  How to use WebUtil\_File\_Get\_Size\_On\_Client\_In\_Bytes\_As\_Number in Forms 11g,  How to use WebUtil\_File\_Get\_Size\_On\_Server\_In\_Bytes\_As\_Number in Forms 11g,  How to use WebUtil\_File\_Get\_Size\_On\_Client\_In\_KB\_As\_Number in Forms 11g,  How to use WebUtil\_File\_Get\_Size\_On\_Server\_In\_KB\_As\_Number in Forms 11g,  How to check if a file exists on client or server using WebUtil
 
## Conclusion
 
In this article, we have shown you how to download and use webutil.pll for Oracle Forms 11g. Webutil is a useful library that enables you to access client-side resources and functionalities when deploying your Forms applications over the web. We hope this article has been helpful for you. If you have any questions or feedback, please let us know in the comments below.
  
## Step 5: Test your webutil functionality
 
To test your webutil functionality, you need to run your form from the web browser. To do this, you need to have a web application server like WebLogic Server installed and configured to run Oracle Forms applications. You also need to have the webutil configuration files in the correct locations on the server and the client. For more details on how to set up webutil for web deployment, refer to the webutil documentation.
 
Once you have everything ready, you can launch your form from the browser by entering the URL of your form in the address bar. The URL should look something like this: `http://:/forms/frmservlet?form=`, where `` is the name of your web application server, `` is the port number of the server, and `` is the name of your form. You should see your form displayed in the browser window.
 
To test your webutil functionality, you can try calling some of the webutil functions and procedures from your form and see if they work as expected. For example, you can try calling `Client_Host('notepad')` to open Notepad on the client machine, or `WebUtil_File.File_Open_Dialog` to open a file dialog on the client machine. You can also check the webutil messages that appear on the status bar of the browser window.
 
## Step 6: Troubleshoot common webutil issues
 
If you encounter any issues while using webutil, you can try some of the following steps to troubleshoot them:
 
- Check the webutil configuration files on the server and the client and make sure they are correct and consistent.
- Check the Java console on the browser window and look for any error messages or exceptions related to webutil.
- Check the Forms server log files on the application server and look for any error messages or exceptions related to webutil.
- Check the JACOB installation and version on the client machine and make sure it is compatible with your Forms version and webutil version.
- Check the security settings of your browser and make sure they allow Java applets and ActiveX controls to run.
- Check the network connectivity between the client machine and the application server and make sure there are no firewalls or proxies blocking the communication.

If none of these steps resolve your issue, you can contact Oracle support or post your question on an online forum for further assistance.
 8cf37b1e13
 
