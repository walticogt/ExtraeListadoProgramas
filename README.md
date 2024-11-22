# ExtraeListadoProgramas

Get-ItemProperty HKLM:\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Uninstall\* | Where-Object { $_.DisplayName -and $_.DisplayVersion } | ForEach-Object { "$($_.DisplayName) - v$($_.DisplayVersion)" } > programas.txt
