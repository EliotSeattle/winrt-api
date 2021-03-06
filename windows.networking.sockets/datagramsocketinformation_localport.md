---
-api-id: P:Windows.Networking.Sockets.DatagramSocketInformation.LocalPort
-api-type: winrt property
---

<!-- Property syntax
public string LocalPort { get; }
-->

# Windows.Networking.Sockets.DatagramSocketInformation.LocalPort

## -description
The local service name or UDP port number associated with a [DatagramSocket](datagramsocket.md).

## -property-value
The local service name or UDP port number.

## -remarks
The [LocalPort](datagramsocketinformation_localport.md) property represents the local service name or UDP port number bound to the [DatagramSocket](datagramsocket.md) object.

An app can set the local service name or UDP port number to use by calling the [BindEndpointAsync](datagramsocket_bindendpointasync.md) , [BindServiceNameAsync](datagramsocket_bindservicenameasync.md), [ConnectAsync(EndpointPair)](datagramsocket_connectasync_13692504.md) , or [GetOutputStreamAsync(EndpointPair)](datagramsocket_getoutputstreamasync_228240991.md) methods on the [DatagramSocket](datagramsocket.md). The bind or connect operation will bind the socket to the specific local IP address and local UDP port number. After the bind or connect operation completes, [LocalAddress](datagramsocketinformation_localaddress.md) property contains the IP address and the [LocalPort](datagramsocketinformation_localport.md) property contains the local UDP port number that the local hostname and service name resolved to.

If the local service name or UDP port number passed to the [BindEndpointAsync](datagramsocket_bindendpointasync.md) , [BindServiceNameAsync](datagramsocket_bindservicenameasync.md), [ConnectAsync(EndpointPair)](datagramsocket_connectasync_13692504.md) , or [GetOutputStreamAsync(EndpointPair)](datagramsocket_getoutputstreamasync_228240991.md) methods is an empty string or the [ConnectAsync(HostName, String)](datagramsocket_connectasync_1841953676.md) or [GetOutputStreamAsync(HostName, String)](datagramsocket_getoutputstreamasync_1619245957.md) method is called, the system will determine the local UDP port to bind to the [DatagramSocket](datagramsocket.md) object.

## -examples

## -see-also
[How to use advanced socket controls ](http://msdn.microsoft.com/library/2e1071d8-a1c7-44c0-b93a-31a701d431c4), [How to use advanced socket controls ](http://msdn.microsoft.com/library/f2c5be73-3461-452e-a38f-d2ddef9b5682), [DatagramSocket](datagramsocket.md), [DatagramSocket.BindEndpointAsync](datagramsocket_bindendpointasync.md), [DatagramSocket.BindServiceNameAsync](datagramsocket_bindservicenameasync.md), [DatagramSocket.ConnectAsync](datagramsocket_connectasync.md), [DatagramSocket.GetOutputStreamAsync](datagramsocket_getoutputstreamasync.md), [LocalAddress](datagramsocketinformation_localaddress.md), [RemoteAddress](datagramsocketinformation_remoteaddress.md), [RemotePort](datagramsocketinformation_remoteport.md)

## -capabilities
ID_CAP_NETWORKING [Windows Phone]
