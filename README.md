<html xmlns="http://www.w3.org/TR/xhtml1/strict">
  <body>
    <h1>Business Object Definition</h1>
    <div>The information contained in this document is the proprietary information of Blue Prism Limited and should not be disclosed to a third party without the written consent of an authorised Blue Prism representative.</div>
    <div>(c) Blue Prism Limited</div>
    <h2>About this document...</h2>
    <div>The Business Object Definition describes the APIs available within a single business object, their parameters and their behaviours from both a business and technical perspective. The definition of each object function describes the business function of the interface, the parameters and usage of the business function and any technical notes required in the on-going support of the interface, including reference to the capabilities of the object. The Business Object Definition API is a dual-purpose document designed to serve the needs of both business users and technical system support staff who require information relating to the business functions available and their details. As such, the BOD is a working document and is subject to change during the course of development and implementation.</div>
    <h2>About Business Objects</h2>
    <div>Business Objects within the environment (i.e. objects which may be drawn onto a process to capture and replicate a part of a business process) adhere to strict guidelines in their implementation. The definition and behaviour of the object both as seen in Process Studio during design time and as implemented during test or via Control Room at runtime uses the same interface definition, known as an object's capabilities. All business objects used within Blue Prism, generic and bespoke, have a common property - Get Capabilities. The GetCapabilities function returns an XML formatted string which defines the interfaces for that object, their friendly names (as they appear in Process Studio) and any inputs and outputs that are required. The Business Object Definition object captures the name, parameters, preconditions and endpoints of each function relating to a business object and translates to the object definition seen within Process Studio.</div>
    <h2>1.0 BluePrism SSH.NET</h2>
    <div>BluePrism SSH.NET is a VBO wrapper for SSH.NET - a Secure Shell (SSH-2) library for .NET</div>
    <p>The runmode of this business object is "exclusive"</p>
    <h3>1.1 Delete File</h3>
    <div>Deletes file from remote directory</div>
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>Host</td>
        <td>In</td>
        <td>Text</td>
        <td>Hostname or IP address of the remote server</td>
      </tr>
      <tr>
        <td>Username</td>
        <td>In</td>
        <td>Text</td>
        <td>Username for the remote server login</td>
      </tr>
      <tr>
        <td>Password</td>
        <td>In</td>
        <td>Password</td>
        <td>Private Key FilePath stored locally</td>
      </tr>
      <tr>
        <td>Private Key FilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Password for the remote server login</td>
      </tr>
      <tr>
        <td>remoteFilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>FilePath on remote server</td>
      </tr>
      <tr>
        <td>Exception</td>
        <td>Out</td>
        <td>Text</td>
        <td>Exception response during execution</td>
      </tr>
    </table>
    <h3>1.2 Download Directory</h3>
    <div>Downloads contents of remote directory</div>
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>Host</td>
        <td>In</td>
        <td>Text</td>
        <td>Hostname or IP address of the remote server</td>
      </tr>
      <tr>
        <td>Username</td>
        <td>In</td>
        <td>Text</td>
        <td>Username for the remote server login</td>
      </tr>
      <tr>
        <td>Password</td>
        <td>In</td>
        <td>Password</td>
        <td>Private Key FilePath stored locally</td>
      </tr>
      <tr>
        <td>Private Key FilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Password for the remote server login</td>
      </tr>
      <tr>
        <td>localFolderPath</td>
        <td>In</td>
        <td>Text</td>
        <td>Folder save location</td>
      </tr>
      <tr>
        <td>remoteFolderPath</td>
        <td>In</td>
        <td>Text</td>
        <td>Remote directory to download</td>
      </tr>
      <tr>
        <td>Exception</td>
        <td>Out</td>
        <td>Text</td>
        <td>Exception response during execution</td>
      </tr>
    </table>
    <h3>1.3 Download File</h3>
    <div>Downloads file from remote server</div>
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>Host</td>
        <td>In</td>
        <td>Text</td>
        <td>Hostname or IP address of the remote server</td>
      </tr>
      <tr>
        <td>Username</td>
        <td>In</td>
        <td>Text</td>
        <td>Username for the remote server login</td>
      </tr>
      <tr>
        <td>Password</td>
        <td>In</td>
        <td>Password</td>
        <td>Private Key FilePath stored locally</td>
      </tr>
      <tr>
        <td>Private Key FilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Password for the remote server login</td>
      </tr>
      <tr>
        <td>localFilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>File save location</td>
      </tr>
      <tr>
        <td>remoteFilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Remote file to download</td>
      </tr>
      <tr>
        <td>Exception</td>
        <td>Out</td>
        <td>Text</td>
        <td>Exception response during execution</td>
      </tr>
    </table>
    <h3>1.4 Execute Command</h3>
    <div>Execute's command on remote server using SSH</div>
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>Host</td>
        <td>In</td>
        <td>Text</td>
        <td>Hostname or IP address of the remote server</td>
      </tr>
      <tr>
        <td>Username</td>
        <td>In</td>
        <td>Text</td>
        <td>Username for the remote server login</td>
      </tr>
      <tr>
        <td>Password</td>
        <td>In</td>
        <td>Password</td>
        <td>Private Key FilePath stored locally</td>
      </tr>
      <tr>
        <td>Private Key FilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Password for the remote server login</td>
      </tr>
      <tr>
        <td>Command</td>
        <td>In</td>
        <td>Text</td>
        <td>SSH Command to run on the remote server</td>
      </tr>
      <tr>
        <td>Response</td>
        <td>Out</td>
        <td>Text</td>
        <td>SSH response after command execution</td>
      </tr>
      <tr>
        <td>Exception</td>
        <td>Out</td>
        <td>Text</td>
        <td>Exception response during execution</td>
      </tr>
    </table>
    <h3>1.5 List FIles</h3>
    <div>Retrieves filenames from remote directory</div>
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>Host</td>
        <td>In</td>
        <td>Text</td>
        <td>Hostname or IP address of the remote server</td>
      </tr>
      <tr>
        <td>Username</td>
        <td>In</td>
        <td>Text</td>
        <td>Username for the remote server login</td>
      </tr>
      <tr>
        <td>Password</td>
        <td>In</td>
        <td>Password</td>
        <td>Private Key FilePath stored locally</td>
      </tr>
      <tr>
        <td>Private Key FilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Password for the remote server login</td>
      </tr>
      <tr>
        <td>remoteDirectory</td>
        <td>In</td>
        <td>Text</td>
        <td>Directory path on remote server</td>
      </tr>
      <tr>
        <td>Exception</td>
        <td>Out</td>
        <td>Text</td>
        <td>Exception response during execution</td>
      </tr>
      <tr>
        <td>Files</td>
        <td>Out</td>
        <td>Collection</td>
        <td>Files in the remote directory</td>
      </tr>
    </table>
    <h3>1.6 Upload File</h3>
    <div>Uploads file to remote server</div>
    <table>
      <tr>
        <th>Parameter</th>
        <th>Direction</th>
        <th>Data Type</th>
        <th>Description</th>
      </tr>
      <tr>
        <td>Host</td>
        <td>In</td>
        <td>Text</td>
        <td>Hostname or IP address of the remote server</td>
      </tr>
      <tr>
        <td>Username</td>
        <td>In</td>
        <td>Text</td>
        <td>Username for the remote server login</td>
      </tr>
      <tr>
        <td>Password</td>
        <td>In</td>
        <td>Password</td>
        <td>Private Key FilePath stored locally</td>
      </tr>
      <tr>
        <td>Private Key FilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Password for the remote server login</td>
      </tr>
      <tr>
        <td>localFilePath</td>
        <td>In</td>
        <td>Text</td>
        <td>Path of local file to upload</td>
      </tr>
      <tr>
        <td>remoteDirectory</td>
        <td>In</td>
        <td>Text</td>
        <td>Remote directory path where the file gets uploaded</td>
      </tr>
      <tr>
        <td>Exception</td>
        <td>Out</td>
        <td>Text</td>
        <td>Exception response during execution</td>
      </tr>
    </table>
  </body>
</html>
