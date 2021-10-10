# ShgardiSocket

Socket 

Connection started in MainTabBarController view didload

- Connection start with URL  with HTTP connection options ( skipNegotiation = true & accessTokenProvider)
	withAutoReconnect in 5 sec 	withHubConnectionDelegate ChatHubConnectionDelegate
	with logging .debug
- .build = > upload to server 

- ReceiveMessage receive massage with on handler      ChatHubConnection append message to message list newMessageAcceptedDelegate  add the message to the list accepted messages 
# events
- OrderRequested
- OrderAccepted
- ConnectionInfo
- OrderStatusUpdated
- UpdateDriverLocation
- InvoiceIssued
- NoDriversFound
- StoreOrderCanceled
- BroadcastDriverLocationMobile
- DismissOrder
- OrderReAssignedBySupport
- CloseOrderBySystem
- OrderCanceledByDriver
- OrderDeliveredConfirmation
- OrderPaidConfirmation
- Confirmation PopUp
- change Donation Amount
- orderDriverChanged 
 
Chat Hub Connection
	+ start
	+ stop
	+ invoke method request
	

chat Hub Connection Delegate

- NewChatHubConnectionDelegate  conform HubConnectionDelegate

		+ connectionDidOpen
			make new socket caller connected 
			invoke request

  		+ connectionDidFailToOpen
			make new socket caller disconnected

		+ connectionDidClose
			make new socket caller disconnected
			if caller should open again => connect socket











