---
title: Change the Style of the Today Cell in Month View
page_title: Change the Style of the Today Cell in Month View | UI for ASP.NET AJAX Documentation
description: Change the Style of the Today Cell in Month View
slug: scheduler/application-scenarios/change-the-style-of-the-today-cell-in-month-view
tags: change,the,style,of,the,today,cell,in,month,view
published: True
position: 5
---

# Change the Style of the Today Cell in Month View



## 

In Month View the Today Cell has the __rsTodayCell__ class applied to it. So changing the style of this cell is possible with the following CSS style:

>note  -Note:- The selector is Skin-dependent. One should replace [skinName] with the name of the currently used Skin.
>


````CSS
	    
	    div.RadScheduler_[skinName] .rsMonthView .rsTodayCell
	    {
	    background-color: #CCFF00;
	    color: #000;
	    border: 1px solid #000;
	    }  
	
````

