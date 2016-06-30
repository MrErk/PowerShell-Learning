# PowerShell Learning

### Structure
* resources - third party scripts, reference articles
* scripts - custom functions which designed for reuse and scripts

### Topics to cover

##### Language Basics
* Get-Help
* Functions vs Scripts
* Cmdlt attribute
* Params attribute
  * pipeline input
  * mandatory params
  * validation
  * dynamic params/$PSBoundItem
* Exception handling
  * ErrorAction
  * try/catch
  * $_.Exception
  * Write-Error vs Throw
* Function Lifecycle: begin/process/end
* Conventions
  * naming
  * use of aliases

##### Foundation commands modules
* File and text manipulation: Get-Content, Get-Child etc
* Discovery: Get-Type, Select-Object -ExpandProperty
* Diagnistics: WMI cs CIM
* SQL:sqpps module

##### Frameworks and advanced tooling
* Desired State Configuration
* Workflows
* Modules
