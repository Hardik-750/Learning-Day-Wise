-listen(Port, callback)

When callback execute?
=> it execute when it is ready to listen user requests.

What is API?
=> An API (Application Programming Interface) is a set of rules and protocols that allows different software applications to communicate and exchange data. It acts as an intermediary or "messenger" that defines how requests are made, what data is exchanged, and how responses are returned, enabling systems to interact without exposing their internal code or underlying architecture. 

API kese create kare?
=> jis bhi method (get/post/patch/put/delete) ko use kare toh ye syntax follow hota he:
                
                -> app.method("/name-your-end-pint", (here you will put a function which help se to execute our task like when we open this end ponit what should we see on the page.))

express ka server ese hi user ki request nhi padh sakta isliye ham below line use karte heapi se pahale:
                -> app.use(express.json()) 
so to read "req.body" we need to use this in express server.