# Tutorials Using AutoIt

AutoIt is a nice scripting language that you can use to automate actions. This is really useful for developing active tutorials. By _active_ I mean tutorials that can work on top of a _live software_. Here is a short AutoIt script which can be executed to show a brief tutorial on how to start the creation dialog.

Those of you who can do a little bit of programming, feel free to use this starting code and make scripts such as this to show what can be done inside TAD Designer Lite. AutoIt works quite linearly – where it would carry out actions inside another software as if someone was actually typing stuff there and moving mouse, pressing keys, etc there.

Also: As AutoIt is a regular programming language too; it can even be used for more sophisticated activities too.

In fact, you could create scripts such as this for useful work too! If you want your office to have a standard set of actions to be performed inside TAD, such scripts could be written to perform those standard actions.

Download AutoIt from [http://autoitscript.com](http://autoitscript.com/)

```
#include <Constants.au3>

;
; AutoIt Version: 3.0
; Language:       English
; Platform:       Win9x/NT
; Author:         Sabu Francis
;
; Script Function:
;   Opens TAD, opens the create objects dialog and shows a baloon tip
;

$tutorTitle = "TAD Tutorial"

; Prompt the user to run the script - use a Yes/No prompt with the flag parameter set at 4 (see the help file for more details)
;Local $iAnswer = MsgBox(BitOR($MB_YESNO, $MB_SYSTEMMODAL), $tutorTitle, "This script will run TAD Designer Lite and walk thru some tutorials. Do you want to run it?")

; Check the user's answer to the prompt (see the help file for MsgBox return values)
; If "No" was clicked (7) then exit the script
;If $iAnswer = 7 Then
;	MsgBox($MB_SYSTEMMODAL, $tutorTitle, "OK.  Bye!")
;	Exit
;EndIf

; Run TDL
;Run("C:\Program Files (x86)\TAD Designer Lite\bin\TadDesignerLite.exe")

; Wait for TAD Designer Lite to become active.
WinWaitActive("[CLASS:TMainForm]")
; Start a new TAD model using Ctrl-N
Send("^n");
; Invoke the creation dialog using Shift-Ctrl-F1
Send("+^{F1}");

; Wait till the dialog pops up
WinWaitActive("[Title:Create objects]")
;MsgBox ( $MB_OK+$MB_TOPMOST, "Now create an object", "Using the creation dialog" &@CRLF &"you can give the starting shape")

Local $sMessage = "Using the creation dialog" &@CRLF &"you can give the starting shape"

ToolTip ( $sMessage, 274,113,"Now create an object", $TIP_INFOICON, $TIP_BALLOON)
Sleep(2000)



; Finished!
```

***

_Press F1 inside the application to read context-sensitive help directly in the application itself_\
_←_ [_∈_](https://docs.teamtad.com/tadtutorial1?do=edit)\
