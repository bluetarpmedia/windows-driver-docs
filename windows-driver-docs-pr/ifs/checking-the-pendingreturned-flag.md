---
title: Checking the PendingReturned Flag
description: Checking the PendingReturned Flag
keywords:
- IRP completion routines WDK file system , PendingReturned flag
- PendingReturned flag
ms.date: 04/20/2017
---

# Checking the PendingReturned Flag


## <span id="ddk_checking_the_pendingreturned_flag_if"></span><span id="DDK_CHECKING_THE_PENDINGRETURNED_FLAG_IF"></span>


If a completion routine does not signal an event, it must check the **Irp‑&gt;PendingReturned** flag. If this flag is set, the completion routine must mark the IRP pending by calling [**IoMarkIrpPending**](/windows-hardware/drivers/ddi/wdm/nf-wdm-iomarkirppending).

 

