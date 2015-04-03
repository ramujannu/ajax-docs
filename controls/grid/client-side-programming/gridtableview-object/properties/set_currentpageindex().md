---
title: set_currentPageIndex()
page_title: set_currentPageIndex() | UI for ASP.NET AJAX Documentation
description: set_currentPageIndex()
slug: grid/client-side-programming/gridtableview-object/properties/set_currentpageindex()
tags: set_currentpageindex()
published: True
position: 5
---

# set_currentPageIndex()



## 

Sets the current page index for the respective __GridTableView__ object. Can be used to control the active page currentlyviewed by the user.

````ASPNET
	        <telerik:RadGrid ID="RadGrid1" runat="server" AllowPaging="True"
	            OnNeedDataSource="RadGrid1_NeedDataSource">
	            <MasterTableView DataKeyNames="OrderID">
	            </MasterTableView>
	        </telerik:RadGrid>
	        <br />
	        <telerik:RadNumericTextBox ID="RadNumericTextBox1" runat="server" MinValue="1" MaxValue="9"
	            Label="Go to page:">
	            <NumberFormat DecimalDigits="0" />
	        </telerik:RadNumericTextBox>
	        <asp:Button ID="Button1" runat="server" Text="Click"
	            OnClientClick="buttonClick(); return false;" />
````



````JavaScript
	            function buttonClick() {
	                var grid = $find('<%= RadGrid1.ClientID %>');
	                var masterTableView = grid.get_masterTableView();
	
	                var value = $find('<%= RadNumericTextBox1.ClientID %>').get_value();
	                if (value != "") {
	                    masterTableView.set_currentPageIndex(value);
	                }
	            }
````

