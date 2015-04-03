---
title: OnDataPagerCreated
page_title: OnDataPagerCreated | UI for ASP.NET AJAX Documentation
description: OnDataPagerCreated
slug: datapager/client-side-programming/events/ondatapagercreated
tags: ondatapagercreated
published: True
position: 1
---

# OnDataPagerCreated



## 

The __OnDataPagerCreated__ client-side event is fired after __RadDataPager__ is created.

The event handler receives one argument:

1. the [RadDataPager object]({%slug datapager/client-side-programming/datapager-object%}) that fired the event.

The following example uses the __OnDataPagerCreated__ event to display a message:

````ASPNET
	    <telerik:RadDataPager ID="RadDataPager1" runat="server">
	        <ClientEvents OnDataPagerCreated="DataPagerCreated" />
	    </telerik:RadDataPager>
````



````JavaScript
	    <telerik:RadCodeBlock ID="RadCodeBlock1" runat="server">
	        <script type="text/javascript">
	            function DataPagerCreated(sender, eventArgs) {
	                alert("Created datapager with UniqueID: " + sender.get_uniqueID());
	            }
	        </script>
	    </telerik:RadCodeBlock>
````



# See Also

 * [OnDataPagerCreating]({%slug datapager/client-side-programming/events/ondatapagercreating%})

 * [OnDataPagerDestroying]({%slug datapager/client-side-programming/events/ondatapagerdestroying%})