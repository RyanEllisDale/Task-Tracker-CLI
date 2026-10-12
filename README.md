# Task Tracker CLI

<picture>
  <source
    srcset="https://github.com/RyanEllisDale/Tasks/blob/main/Docs/Tasks%20Title%20Dark%20Theme.jpg"
    media="(prefers-color-scheme: dark)"
  />
  <source
    srcset="https://github.com/RyanEllisDale/Tasks/blob/main/Docs/Tasks%20Title%20Bright%20Theme.jpg"
    media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)"
  />
  <img src="https://github.com/RyanEllisDale/Tasks/blob/main/Docs/Tasks%20Title%20Bright%20Theme.jpg" />
</picture>

Task Tracker CLI is a small program made for the Windows CLI, I developed it as a Terminal based alternative to having notepad glued to my screen at all times. It is a lot simpler than notepad, having only one Task file that automatically generates and saves as the program runs through its life-cycle. Sadly for now this project is Windows only as I have not configured it's AppData to work across alternative operating systems such as Linux or Mac OS, in the future this is something I would like to add. 

## Installation 

* To install the project please [download](https://github.com/RyanEllisDale/Task-Tracker-CLI/releases) or compile a .exe with an appropriate name
* Add the folder that the .exe is located in to your systems PATH environment variable
  * Control Panel » System and Security » System » Advanced System Settings » Environment Variables.
* Then test the application by running any command, Recommended : "Hello"
  <pre> PS C:\Users\Local_User> <mark> &lt;.exe Name&gt; Hello </mark> </pre>

> [!TIP]
> For a more comprehensive view please visit the [Installation Wiki](https://github.com/RyanEllisDale/Task-Tracker-CLI/wiki/Installation)

## Usage

Basic Syntax is : &lt;.exe Name&gt; &lt;Command Name&gt; &lt;Command Argument 1...&gt; &lt;Command Argument 2...&gt;

Here is a few of the common available commands :
**Adding First Task Example :**
<pre>
PS C:\Users\Local_User> <mark> tasks </mark> <mark> add </mark> <mark> "Hello Task Tracker CLI" </mark> <mark> In-Progress </mark>
Task: hello task tracker cli was Successfully added
</pre>

**Listing All Current Tasks :**
<pre>
PS C:\Users\Local_User> <mark> tasks </mark> <mark> list </mark>
0 : hello task tracker cli : In Progress : Mon 10/12/26 02:14:51 : Mon 10/12/26 02:14:51
</pre>

**Printing Full Details of Task :**
<pre>
PS C:\Users\Local_User> <mark> tasks </mark> <mark> print </mark> <mark> 0 </mark>
----------
Task: hello task tracker cli
ID : 0
Status : In Progress
Created At: Mon 10/12/26 02:14:51
Updated At: Mon 10/12/26 02:14:51
----------
</pre>

**Deleting First Task Example :**
<pre>
PS C:\Users\Local_User> <mark> tasks </mark> <mark> delete </mark> <mark> 0 </mark>
Task : hello task tracker cli was Successfully delted
</pre>

> [!TIP]
> For a more comprehensive view please visit the [Usage Wiki](https://github.com/RyanEllisDale/Task-Tracker-CLI/wiki/Usage)

## Licensing 

This project itself is available freely for anyone to use how they like but this project makes use of Lohmann, N's JSON for Modern C++ under the MIT License.

> [!TIP]
> For a more comprehensive view and full licensing of Lohmann, N's JSON for Modern C++ please visit the [Usage Wiki](https://github.com/RyanEllisDale/Task-Tracker-CLI/wiki/Attribution)

