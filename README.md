# CheckPlease
## Target your payloads.
The go-to repository for the newest targeted payload and sandbox-detection modules.

Every module functions as a standalone "check." All checks can be run like so:

```
<language> <module_name> <optional argument>
```

This repository is for defenders to harden their sandboxes and AV tools, malware researchers to discover new techniques, and red teamers to get serious about their paylaods.

I want you to **contribute** to this repository to make it truly comprehensive. If your implementation works, I will merge your modules into this repository within **one day**. 


## Examples 

**PowerShell**: Check that the parent process of your payload was WinWord.exe:

```
PS arvanaghi: .\parent_process.ps1 WinWord
```

**Python**: Make the user click 6 times before executing your payload:

```
arvanaghi: python click_tracker.py 6
```

**Go**: Ensure user activity by making the user click a pop-up prompt before executing your payload:

```
arvanaghi: go run user_prompt.go "This is the box title" "This is the box message." 
```

**Ruby**: Ensure there have been at least 4 USB devices ever mounted on the system:

```
arvanaghi: ruby usb.rb 4 
```

**Perl**: Make your payload execute on a certain date.

```
arvanaghi: perl date_trigger.pl 09/20/2017
```

You know how to run **C** and **C#** code.

## Why every language?

Payloads are more commonly being delivered in languages that are not C. In implementing in every language, we give sandbox and antivirus vendors a broader scope from which to detect. In your red teams, any payload you deliver can now be more targeted. 

