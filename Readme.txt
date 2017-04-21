在 Windows 8 /WIN10【桌面】出現【家用群組】，該如何刪除？


資料來源:https://dotblogs.com.tw/chou/archive/2012/12/27/86051.aspx


問題的解決方法

1. 先嘗試做 [重新整理]，在看看 [家用群組] 是否還在。

2. 如果還在的話，開啟記事本，將以下內容複製到記事本中，並另存成 remove.reg 檔案。

Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\HideDesktopIcons\NewStartPanel]
"{B4FB3F98-C1EA-428d-A78A-D1F5659CBA93}"=dword:00000001

[HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\HideDesktopIcons\ClassicStartMenu]
"{B4FB3F98-C1EA-428d-A78A-D1F5659CBA93}"=dword:00000001

[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\HideDesktopIcons\NewStartPanel]
"{B4FB3F98-C1EA-428d-A78A-D1F5659CBA93}"=dword:00000001

[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\HideDesktopIcons\ClassicStartMenu]
"{B4FB3F98-C1EA-428d-A78A-D1F5659CBA93}"=dword:00000001