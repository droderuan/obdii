# obdii

The information system inside a car has basically two core parts: CAN bus and OBD-II. 

### Controlled Area Network - CAN bus
The CAN bus is a protocol which defines how the sensors and others parts of the car, or ECU's (eletronic control units), will share data between the car. This is build using two cables connecting all the ECU's and then each ECU can connect to other.
The car can have many ECU's, from the engine to sensors in the backseat.

https://www.webautomotivo.com.br/tag/programar-rede-can/

### OBD-II - On-board Diagnostic II
On the top of CAN bus, is the OBG-II and this protocol is responsible to take the CAN bus data and transforms into a common API to share data about the current state of the car. There is a fews categories including historical data, current data, diagnostics about issues, etc.
The OBD-II has a connector where we can connect a device to start gathering some data.
#### PIDS
The OBD protocol stream different types of data, which differs based on a identifier code, this identifier code is called *pid*. The types of pids and when is available or not, depends on the model and the manufacture.
OBD-II allows only to read data from the car, using a analogy, it works like a web server, where we ask for a resource using the url, in this case a pid, and, if exist, the serve returns the resource, the car returns the related information.

Reference:

* Playlist about CAN bus and  OBD-II: https://www.youtube.com/watch?v=oYps7vT708E&list=PLpV68vjf4Xo4vZ_SjJ6tTlomYm-k18vDZ
* React Native with OBD2: https://star.global/posts/react-native-for-automotive/
