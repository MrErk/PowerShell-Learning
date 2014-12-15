# Gotchas, tricks and other less obvious PowerShell features

#### Discovery
* Get-Help < command name > (gets basic command information)
* Get-Help < command name > -full (gets all command information)
* Get-Help about_< reserved word > (gets information about keyword) e.g. Get-Help about_Throw

#### Syntax
* Executing scripts from a script or function: Invoke-Expression (&) or Invoke-Command

##### Strings
* Double quotes will evaluate expressions, single quotes are literals e.g.
```
$Something = 'foo'
$EvalText = "This will evaluate $Something"
$LiteralText = 'This will not evaluate $Something'
Write-Host $EvalText     #output: This will evaluate foo
Write-Host $LiteralText  #output: This will not evaluate $Something
```
* Backtick is the escape character e.g. `n = new line
* Composite string formatting uses -f
```
"Today is {0}" -f (Get-Date) #output: Today is 15/12/2014 9:06:38 AM
"Today is {0:d}" -f (Get-Date) #output: Today is 15/12/2014
```
