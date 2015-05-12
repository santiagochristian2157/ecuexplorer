# Introduction #

Brief description of the SSM protocol specification used by ecuExplorer


# Details #

The SSM protocol is relatively simple and because of this its very easy to use.  It is quite an old protocol and therefore has some draw-backs, the worst being that it only operates at a 4800 baud.  None-the-less sample rates can be achieved as quickly as 150ms with 4 items being requested. The more data items you request to be sent back the slower the sample rate gets. This should provide 6.66 samples / second.  Realistically its not comparable to some of the other systems available and you’re sure to miss some of the finer data transitions if you’re logging for tuning purposes but it does provide a decent level of diagnostics logging.

The SSM protocol seems to be fairly low on the priority list of the ECU and I encountered some response problems when the vehicle was put under high stress like full-throttle runs.  To counter these just make sure that your receive routine is able to deal with partial data and response data that never comes through.