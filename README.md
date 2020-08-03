<H1>Introduction to PProAPI</H1>
<p>The PPro API is a WEB based application programming interface which allows traders at Day Trade The World to create various custom trading tools that augment and integrate with the Ralota trading platform used by the firm. This allows the trader to create real-time trading apps to assist in various trading activities. The following are some of the examples of trading tools that a trader may want to develope to assist in my trading strategies: 
<li>Order and Rrisk Management</li>
<li>Closing Imbalance and Closing Auction performance for various markets</li>
<li>Real-time Feed Readers to collect level 1 and level 2 quotes for trading data analysis</li>
<li>Real-time monitoring of time of sale prints for price and volume</li>
<li>Consolidate feeds (Level 1, Level 2, Time Of Sale, OrderStatus into a consolidated feed</li>
<li>Create algorithmic trading bots that monitor the market and execute trading strategies</li>
</p>
<H2>Technical Overview of API frameworrk</H2>
<p>The API requires that the Ralota Trading Platform be installed on your PC and that you have a valid user account and password setup. This is not a standalone API library and must integrate to the Ralota trading platform while it is running to allow REST API calls to provide various trading services. Due to the way this product is architected the trading platform must always be running in order to use the API and it does not require any user authentication because this is provided through the trading platform's user authentication process.</p>
<H3>How to Setup</H3>
<li>Install Ralota Trading Platform on PC</li>
<li>Enable API through your trading supervisor</li>
<li>Develop and Test API in TMS</li>
<H3>General Structure of the API</H3>
<p>The API is structured to allow traders and programmers a interface to code custom trading applications that integrate into the Ralota trading platform. The API can be divided into two set of trade process flows:</p>

<li>Trade Data Services</li>
<li>Realtime L1 Data Feed</li>
<li>Realtime L2 Data Feed</li>
<li>Realtime Time Of Sale (TOS) Feed</li>
<li>TSX Static Imbalance Feed</li>
<li>NYSE & NASDAQ Realtime Opening and Closing Imbalance</li>

<p>The data services component of the API allows users to subscribe and direct trade data output to a data repository or collect data in realtime using the trading platforms UDP broacasting mechanism. The following are the API calls that would be used when creating the above trade applications:</p>
  
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


<li>Order and Trade Management</li>

<p>The Order and Trade Management services component of the API allows users to subscribe and direct trade order and trade data output to a data repository or collect data in realtime using the trading platforms UDP broacasting mechanism. The following are some data services that can be created using the API:

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

<H4>General Workflow Structure of the API</H4>  
</p>The followinga are some simple workflow models:,/p>


<H3>API Functions</H3>

<p>The following is a the entire list of functions that make up the API:</p>

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

<H3>Trade Workflow Process</H3>
<p>In order to use the API properly you must understand the general workflow process for create trading tools or data models with the Ralota Trading platform. The following outlines the general worklow steps:
<li>Register Security for specific trade data (L1, L2, TimeOfSale, OrderStatus, OrderEvent)</li>
<li>SetOutput for the security data (To A file or Realtime UDP broacasts)</li>
<li>If the output is to a file then create batch functions to process the data in the file</li>
<li>If the output is realtime UDP broadcasts then use a realtime UDP library to read the data off the port(s)</li>
<li>Process data from realtime port(s) or process data from file</li>

<p>The following two API calls setup the various securities for specific trade data and then route the output to a file or UDP port number:
  
<li>Register</li>
<li>SetOutput</li>
</p>




