# BHPC-Manager
It's a one-stop center to oversee a significant portion of the procedures related to the distribution process of our foreign partner's products in Europe and Latin America.
The currently operational functions (albeit in testing) include:
- Guided procedure for saving a sales or sampling order (orders related to supplies can also be registered, but some fields are still inconsistent).
- Ability for the user to input products related to sales/sampling, specifying selling price or if they are F.O.C. (free of charge).
- Once the products are loaded into the order, it is possible to automatically generate the main documents: PROFORMA INVOICE, PACKING LIST, and MULTIMODAL FORM.
- Finally, it will be possible to track the order status and numerous other (mostly logistical) parameters useful at the time of drafting periodic reports to be presented to the partner.

At present the application is still in working progress but can already be used to create a consistent dataset of outgoing orders (sales and sampling) and to quickly create documentation (avoiding manual creation, slow and fallacious).

FUNCTIONS STILL TO IMPLEMENT
- Inventory Tracking: Record the stock levels. Register the values of the last inventory. By entering all incoming and outgoing movements, stock availability should always be up to date. This would allow the application to provide real-time information to management about availability.

- Currency management: Create a way to handle order in different currency

- Supplies: Register the supplies in a consistent way


BHPC MANAGER 1.5
First version stable enough and testable even by third-party users. Below I will describe the working functions of the application.
The application consists of 5 main TABs that allow you to navigate through the main functions.

CONTROL BOARD - A control center for incoming and outgoing shipments of BHPC products.
SHIPMENT DETAILS - A panel where you can view and modify the logistical and generic details of an order.
ORDERED PRODUCTS - Panel where you can enter and/or view the products belonging to the selected order.
WAREHOUSE (not yet available)
ADMINISTRATION - Some simple administration functions such as selecting the data saving folder.
SYNCHRONIZATION SYSTEM (Still in testing phase, but seemingly functional)

The Excel application is designed to be used as a client that connects to a "database server" to work with data. This approach is very useful because it allows multiple users to simultaneously use their own copy of the client and manipulate the data on the server, always with updated data (also from other users).

NOTE: there's also a version of the application without data synchronization system. This version is easier to manage and is recommended for those who do not work in teams.

From the control board, it is possible to perform manual synchronizations which currently include syncing:
Orders, order_data file.
Products of orders, sales_data file.
Customers, client_lookup table.
A time synchronization system has also been implemented, preset to a 3-minute delay between updates.
Finally, whenever a user performs operations that modify the client-side datasets, the same changes are reflected in the server-side files to make them available to all other users.

CONTROL BOARD
Allows tracking of BHPC orders both incoming and outgoing.
The table allows filtering shipments by:
Customer
Order status
It should provide order managers with greater awareness of what is happening and what needs to be done.

ORDER DETAILS
Here you can enter any detail related to the order.
Consequently, it is also possible to retrieve this information in a user-friendly interface (UI changes to the ORDER DETAILS tab are planned for upcoming releases).
There are a series of NOTE cells that allow the user to take notes and link them to the order so that nothing is forgotten.
A status bar has been implemented to provide an immediate view of the order status, what has already been done, and what still needs to be done before shipping.

ORDERED PRODUCTS
- In this section, there is an entry form for entering the references ordered by customers or those received from the supplier.
- It has been designed to be as user-friendly as possible while also considering the possibility of products sold at full price, others at discounted prices, and still others free of charge (FOC).
- It is possible that further improvements will be implemented in the future to make the entry of new shipments even more immediate.


bhpc_manager_v1.2.xlsm

This is the file with data and client all in one file. Much more reactive and efficient. Best solution for solo workers.
