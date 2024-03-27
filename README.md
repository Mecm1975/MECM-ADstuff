This report will not work until you extend your hardware inventroy with the required WMI classes.  Example
  #Write-Host "Checking Battery Specs"
	 (Get-WmiObject -Class "BatteryStaticData" -Namespace "ROOT\WMI").DesignedCapacity
	 (Get-WmiObject -Class "BatteryFullChargedCapacity" -Namespace "ROOT\WMI").FullChargedCapacity
   (Get-WmiObject -Class "BatteryCycleCount" -Namespace "ROOT\WMI").CycleCount
	  
