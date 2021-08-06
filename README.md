# Set version on AssemblyInfo.cs GitHub Action for Windows runners
Set the version in all the AssemblyInfo.cs or AssemblyInfo.vb files in any subdirectory. For use with .NET Full Framework projects.

## Usage

```yml
- name: Set version on AssemblyInfo.cs
  uses: dannevesdantas/set-version-assemblyinfo-win@v1.0.0
  with:
    version: '3.2.0'
```

## Specifying folder path
You can specify an optional folder path to search for AssemblyInfo.cs/.vb files. The default value is ${{ github.workspace }}

```yml
- name: Set version on AssemblyInfo.cs
  uses: dannevesdantas/set-version-assemblyinfo-win@v1.0.0
  with:
    version: '3.2.0'
    path: '${{ github.workspace }}/MyProject/App'
```

## Requirements
This GitHub Action is compatible with Windows based runners only.

# Credits

Thanks [cheeso](http://social.msdn.microsoft.com/profile/cheeso/) for providing the PowerShell [SetVersion.ps1](https://web.archive.org/web/20151112002214/http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-components-postattachments/00-08-41-04-10/SetVersion.ps1) script at [MSDN Blogs](http://blogs.msdn.com/b/dotnetinterop/archive/2008/04/21/powershell-script-to-batch-update-assemblyinfo-cs-with-new-version.aspx), still available at [Wayback Machine](https://web.archive.org/web/20151112002214/http://blogs.msdn.com/b/dotnetinterop/archive/2008/04/21/powershell-script-to-batch-update-assemblyinfo-cs-with-new-version.aspx).

# License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
