# CodeReference
Simple code reference for convert type in Apex and JavaScript

Convert List value to Set of ids \n
 
 System.debug('The number of Cases'+MyCaseList.size());    
    List<Case> CaseList =[select id from Case ];
    Set<Id> CaseIds = (new Map<Id,Case>(CaseList)).keySet();
    System.debug('The total case id is ' + CaseIds.size());
