# PowerShell-Message-Boxes-WPF
Quick inline PowerShell tutorial to use GUI Message Boxes in PowerShell...

## Prerequisites
- This sample Uses the .NET System.Windows.Messagebox .NET class to display message boxes More information in the following link (right-click and choose "Open in a new tab" for now to keep a tab on this page, as the **a href=https://blabla target="_blank"** thingy doesn't work on ReadMe.md on Github for now:
<a href="https://docs.microsoft.com/en-us/dotnet/api/system.windows.messagebox?view=netframework-4.8" target="_blank">System.Windows.MessageBox class description</a>


- Before being able to use the System.Windows.MessageBox .NET class, you must load the PresentationFramework.dll .NET assembly (an assembly is a sort of library of functions)

```powershell
Add-Type -AssemblyName presentationframework
```

## Using the .NET MessageBox class directly in Powershell
- To use the MessageBox class to create a Message Box in powershell, we are just using the following format:

```powershell
[.NET class]::Method()
```

for example, to show a box, we will call the .NET class System.Windows.MessageBox, with the "Show()" method:

```powershell
[System.Windows.MessageBox]::Show($msg,$Title, $Button, $icon)
```

See the .PS1 file comments and examples for a bit more details, and more importantly, have fun !
