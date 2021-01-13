# SSH.NET
This is a VBO wrapper for SSH.NET which is a Secure Shell (SSH) library for .NET, optimized for parallelism. The source code of SSH.NET can be found at https://github.com/sshnet/SSH.NET

## Usage
The asset provides following actions. Further actions may be added in the future

* **Delete File**
* **Download Directory**
* **Download File**
* **Execute Command**
* **List Files**
* **Upload File**

## Configuration
* Download or clone this repository. Extract the *.bprelease file* and import it into your Blue Prism environment
* Copy Renci.SshNet.dll to C:\Program Files\Blue Prism Limited\Blue Prism Automate or your BluePrism installation directory

## Actions
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

## Help

If issues are encountered, please submit a new issue on the Issues tab for this repository:

https://github.com/blue-prism/SSH.NET/issues
