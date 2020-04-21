@Save following code as .bat.
@Double click .bat to remove all empty folder。
@pause
@echo clean disk c
dir c: /ad /b /s |sort /r >>c:kill.txt
For /f %%i in (c:kill.txt) DO rd %%i
echo y |del c:kill.txt
@echo  clean disk D
@pause
dir d: /ad /b /s |sort /r >>d:kill.txt
For /f %%i in (d:kill.txt) DO rd %%i
echo y |del d:kill.txt
@echo clean disk E
@pause
dir e: /ad /b /s |sort /r >>e:kill.txt
For /f %%i in (e:kill.txt) DO rd %%i
echo y |del e:kill.txt
@echo All done, Thanks for using!
