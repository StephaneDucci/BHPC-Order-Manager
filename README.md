# Perfumes Orders Manager

APPLICATION PREVIEW **https://youtu.be/yMHvTjarY9U**

**Perfumes Orders Manager** is a comprehensive solution for overseeing a substantial part of the procedures involved in the distribution of our foreign partner's products across Europe and Latin America.

---

## Changelog

[5.2] - 2024-12-28

Fixed

Minor Bug Fixes and Exception Handling: Addressed several minor bugs and resolved small exceptions that previously caused errors.

Improved

Intrastat Value Calculation: Completely revamped the calculation of Intrastat values. The results are now error-free and capable of handling any type of gift set, provided the product master data is properly maintained.

Data Visualization: Improved data display using a ListBox for enhanced clarity and usability.

### [5.1] - 2024-12-08
#### Added
- **Cell Protection Toggle**: Added the ability to lock and unlock protected cells, providing users with greater control over data editing and security.

#### Fixed
- **Minor Bug Fixes**: Resolved several minor bugs to improve system stability.

---

### [5.0] - 2024-11-04
#### Added
- **Complete Product Management through GUI**: Easily manage product logistics details with an intuitive graphical interface designed for user convenience.
- **Comprehensive Bill of Materials Management for Composite Products (Giftsets)**: Fully manage the bill of materials for composite products.
- **Risk Class Management for Hazardous Products**: Complete risk class management for products classified as hazardous.
- **Enhanced Autonomy for Non-Technical Users**: Tools enabling users without VBA or programming knowledge to create products and/or giftsets without breaking the document creation code, including the Multimodal form for hazardous goods.

#### Improved
- **User Interface**: A visually appealing, intuitive, and consistent UI theme.

#### Optimized
- **ADMIN Section**: Fully optimized with new commands for data import/export/deletion.
- **Database Reset Capability**: Users can now rebuild the database from scratch.

#### Fixed
- **Minor Bug Fixes**: Resolved several minor bugs to improve stability.

---

### [4.1] - 2024-07-20
#### Added
##### Order and Shipment Control Features:
- **Order Creation**: Create sales, sampling, and supply orders.
- **Product Line Input**: Add products to orders, specifying if they are for sale, discounted, or offered as F.O.C. (free of charge).
- **Shipment Details Userform**: A dedicated userform to view details of each shipment (whether supply, sampling, or sales), allowing users to save all logistical details, preparation status, payment status, import/export document drafting status, and additional notes.
- **Currency Conversion**: Convert orders in foreign currencies to euros.
- **Automatic Document Generation**: Automatically generate key documents for customers and transporters, including:
  - Invoice
  - Packing List
  - Multimodal Form

##### Warehouse Control Features:
- **Warehouse Section**: Added a dedicated section to track product movements within the warehouse.
- **Product Management Userform**: Userform for managing Perfumes products:
  - Create or modify products.
  - Create/modify bill of materials (BOM) for composite products, such as gift sets.
  - Define and assign risk classes to hazardous products for correct automatic generation of multimodal forms.
- **Production Management**: Execute production orders and preview production to check the availability of all necessary components for composite products.
- **Stock Availability Tracking**: Track product availability in the warehouse to quickly determine if customer demands can be met.
- **Gift Set Production**: Implemented functionality to execute the production of gift sets.

##### Administration Features:
- **Administration Section Update**: Completely updated the administration section.
- **Data Import/Export**: Allow users to export and import data as needed.
- **Database Access**: Allow users direct access to databases for making corrections directly to records.

##### Customers/Suppliers Features:
- **Customer/Supplier Management Userform**: Implemented a userform to create or modify customer and supplier details.

---

## Future Features (Planned for Future Versions)
- **Migration to Access Database**: Transition to an Access database to support multi-user functionality and facilitate data access (read/write) for large datasets.
- **Bug Fixes and Exception Handling**: Implement comprehensive bug fixes and exception management to enhance system stability. *(Completed in v5.0)*
- **UI/UX Improvements**: Enhance the user interface and experience for greater intuitiveness and efficiency. *(Completed in v5.0)*
- **Product Management Enhancements**: Include warehouse details (e.g., stock levels, average cost) in the product management userform. *(Completed in v5.0)*

---

## Status and Usage

The application is fully functional and can be used efficiently for the following sections:

- **HOME**: Create, modify, and delete supply and sales orders.
- **BASKET**: Manage order contents, including the production of composite products (giftsets).
- **WAREHOUSE**: Track warehouse operations, including incoming and outgoing stock movements.
- **DOCS**: Generate sales documentation, including invoices, packing lists, and multimodal forms for hazardous goods.

> **Note**: The **REPORTING** section is currently under development and remains a work in progress.


The **Perfumes Orders Manager** is continuously evolving to provide a better experience for users and address the growing needs of the business.
