# How to enable gpedit.msc into windows 10 or 11

### Example:(Windows 10 Home) ###

<h6>Solution:</h6>


+ Open Command Prompt with  run as administration
<h6>Command Prompt(CMD)Command</h6>

+ FOR %F IN ("%SystemRoot%\servicing\Packages\Microsoft-Windows-GroupPolicy-ClientTools-Package~*.mum") DO (
DISM /Online /NoRestart /Add-Package:"%F" )


+ FOR %F IN        ("%SystemRoot%\servicing\Packages\Microsoft-Windows-GroupPolicy-ClientExtensions-Package~*.mum") DO (
DISM /Online /NoRestart /Add-Package:"%F" )


![Screenshot (64)](https://user-images.githubusercontent.com/69615463/137346363-be5a84c6-1d45-4468-aa1f-0ecd9298f1ee.png)

+ Press  key win + r

![Screenshot (65)](https://user-images.githubusercontent.com/69615463/137346513-52927107-5d31-41aa-9b4d-9edf8559f9cc.png)


+ Type gpedit.msc and press enter key

![Screenshot (66)](https://user-images.githubusercontent.com/69615463/137346697-bd8a0eb7-4e30-4aa5-af50-ac1e94402186.png)