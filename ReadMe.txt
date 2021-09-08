What is VBC6.EXE?
-----------------

VBC6.EXE is a utility designed to fix License problems with ActiveX 
Controls that ship with Microsoft Visual Basic 6.0.  The utility will 
not fix third party controls, or controls not normally installed by 
Microsoft Visual Basic 6.0.  

VBC6.EXE will help correct problems with the following symptoms:

Symptom I
---------

When trying to site a control within a project, Microsoft Visual Basic raises the following 

error dialog:

   License Information For This Component Not Found.  You Do Not Have An
   Appropriate License To Use This Functionality In The Design Environment.

Symptom II
----------

When trying to compile a project, Microsoft Visual Basic raises the following error dialog:

   Compile Error : Permission Denied

Symptom III
-----------

When using the Application Wizard, Microsoft Visual Basic raises an error dialog similar to:

   60: Method ~ of Object ~ failed

Symptom IV
----------

When trying to run a project, Microsoft Visual Basic raises the following error dialog:

   Runtime Error '429' : ActiveX Component Can't Create Object

Which ActiveX controls does VBC6.EXE work with?
-----------------------------------------------

The following is a list of ActiveX controls that VBC6.EXE is aware of.
ActiveX Control                     FileName        Version      Edition
------------------------------------------------------------------------

ADO Data Control 6.0                 MSADODC.OCX    6.00.8171    L,P,E
Chart Control 6.0                   MSCHRT20.OCX    6.00.8177      P,E
Comm Control 6.0                    MSCOMM32.OCX    6.00.8169      P,E
Common Dialog Control 6.0           COMDLG32.OCX    6.00.8169    L,P,E
Data Bound List Controls 6.0        DBLIST32.OCX    6.00.8169    L,P,E
DataGrid Control 6.0                MSDATGRD.OCX    6.00.8169    L,P,E
DataList Controls 6.0               MSDATLST.OCX    6.00.8169    L,P,E
DataRepeater Control 6.0            MSDATREP.OCX    6.00.8169      P,E
FlexGrid Control 6.0                MSFLXGRD.OCX    6.00.8169    L,P,E
Hierarchical FlexGrid Control 6.0   MSHFLXGD.OCX    6.00.3005    L,P,E
MAPI Controls 6.0                   MSMAPI32.OCX    6.00.8169      P,E
Masked Edit  Control 6.0            MSMASK32.OCX    6.00.8169      P,E
Multimedia Control 6.0                 MCI32.OCX    6.00.8169      P,E
PictureClip Control 6.0             PICCLP32.OCX    6.00.8169      P,E
RemoteData Control 6.0               MSRDC20.OCX    6.00.8169        E
Rich Textbox Control 6.0            RICHTX32.OCX    6.00.8169    L,P,E
SysInfo Control 6.0                  SYSINFO.OCX    6.00.8169      P,E
Tabbed Dialog Control 6.0           TABCTL32.OCX    6.00.8169    L,P,E
Windows Common Controls-3 6.0       COMCT332.OCX    6.00.8169      P,E
Windows Common Controls 5.0 (SP2)   COMCTL32.OCX    6.00.8022    L,P,E
Windows Common Controls 6.0         MSCOMCTL.OCX    6.00.8177    L,P,E
Windows Common Controls-2 5.0 (SP2) COMCT232.OCX    6.00.8022    L,P,E
Windows Common Controls-2 6.0       MSCOMCT2.OCX    6.00.8177    L,P,E
Winsock Control 6.0                 MSWINSCK.OCX    6.00.8169      P,E

L = Learning Edition
P = Professional Edition
E = Enterprise Edition

How do I use VBC6.EXE?
----------------------

VBC6.EXE requires that the Microsoft Visual Basic 6.0 run-time engine is
 installed on the system where the utility is going to be used.  The 
run-time engine is available on the Microsoft Visual Basic 6.0 (or Visual
 Studio 6.0) under the \Common\Tools\VB\Cabinets directory.  The 
VBRUN60.CAB contains a self extracting EXE which will installed the 
Microsoft Visual Basic 6.0 run-time engine onto your machine.

Before running the VBC6.EXE utility, make sure there are no other 
applications running.

Simply double click on VBC6.EXE through the Windows Explorer.  The utility 
will attempt to detect Microsoft Visual Basic 6.0, and will installed the 
required Licenses for the Edition detected.

If successful, you will see a dialog box similar to the following:

"Enterprised Design Licenses Have Been Installed Successfully"

VBC6.EXE also offers a silent mode.  Running the VBC6.EXE from the command 
with a "/q" will run the utility without any user interface.  Result codes 
can be captured and used by other apps to test if the Licenses were installed.

Result Codes And Error Messages
-------------------------------

Exit Code 0   : Licenses for that Edition where installed
Exit Code 1   : Microsoft Visual Basic 6.0 was not detected on this system
Exit Code 2   : Could Not Load A Support Utility Library
Exit Code 3,4 : At Least 1 Design License Was Not Properly Installed
Exit Code 5   : Unable To Install Any Design Licenses
Exit Code 6   : There Was An Unspecified Error With The VBC6 Utility

Disclaimer
----------

The utility discussed in this article is provided "as is" and Microsoft does not guarantee that it can be used in all situations. Although Microsoft support engineers can help with the use of this product, it is not supported. Use this tool at your own risk.