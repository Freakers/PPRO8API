<H1>Introduction to PProAPI</H1>
<p>The PPro API is a WEB based application programming interface which allows traders at Day Trade The World to create various custom trading tools that augment and integrate with the Ralota Trading platform used by the firm. This allows the trader to create various real-time trading tools to assist in various trading tasks. The following are some of the examples of trading tools that I require to assist in my trading strategies: 
<li>Order and Rrisk Management</li>
<li>Closing Imbalance and Closing Auction performance for North American and European Markets</li>
<li>Real-time Feed Readers to monitor level 1 and level 2 quotes</li>
<li>Real-time monitoring of time of sale prints for price and volume</li>
<li>Consolidate feeds (Level 1, Level 2, Time Of Sale, OrderStatus into a consolidated feed</li>
<li>Create algorithmic trading bots that monitor the market and execute trading strategies</li>
</p>
<H2>Overview of API</H2>
<p>The API requires that the Ralota Trading Platform be installed on your PC and that you have a valid user account and password setup. This is not a standalone API library and must integrate to the Ralota trading platform while it is running to allow API calls to be routed to the back end servers to provide real-time trading. Due to the way this product is architected the trading platform must always be running in order to use the API and it does not require any user authentication because this is provided through the trading platform's user authentication process.</p>
<H3>How to Setup</H3>
<li>Install Ralota Trading Platform on PC</li>
<li>Enable API through your trading supervisor</li>
<li>Develop and Test API in TMS</li>
<H3>General Structure of the API</H3>
<p>The API is structured to allow trading proffessional and programmers a interface to code custom trading applications that integrate into the Ralota trading platform. The API can be divided into two set of trade process flows:</p>
<li>Trade Data Services</li>
<li>Order and Trade Management</li>
<p>The data services component of the API allows users to subscribe to various forms of trade data and collect and disseminate that data into various forms of trade data services:
<li>Realtime L1 Data Feed</li>
<li>Realtime L2 Data Feed</li>
<li>Realtime Time Of Sale (TOS) Feed</li>
<li>TSX Static Imbalance Feed</li>
<li>NYSE & NASDAQ Realtime Opening and Closing Imbalance</li>
<li>Realtime Order Status and Events</li></p>
<H4>Order and Trade Management</H4>
<H4>General Structure of the API</H4>  
</p>
<H3>API Calls</H3>
<p>The API uses a symbol registration and output process to subscribe to trading data services (L1, L2, TOS, OrderStatus, OrderEvents, TraderInfo, etc..) and also provides a mechanism to send orders to the trading floor via a rest call. The following is a overview of the API calls:
<li>Register</li>
<li>SetOutput</li>
<li>GetSnapshot</li>
<li>Deregister</li>
<li>GetEnvironment</li>
<li>Get</li>
<li>GetBlotterSnapshot</li>
<li>GetLv1</li>
<li>GetTraderInfo</li>
<li>GetTransactions</li>
<li>ExecuteOrder</li>
<li>ExecuteBasketOrder</li>
<li>ExecuteListOrder</li>
<li>CancelOrder</li>
<li>CancelOrderReplace</li>
<li>GetOrderNumber</li>
<li>GetOrderState</li>
<li>GetOpenOrders</li>
<li>SendTrailingStop</li>
<li>SendSwiftStop</li>
<li>GetOpenPositions</li>
<li>Flatten</li>
</p>
<H3>Official PPro8 PProAPI Wiki  Page</H3>
<p>The following is the wiki page created by DTTW documenting all the various API calls and examples of some of the APIs. URL: https://www.daytradetheworld.com/wiki/pproapi/
</p>


