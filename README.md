# Shopbridge_Base
This repository contains a .Net 5 and C# solution, which contains the following API action methods that can be consumed by the front end applications.
1. GetAllProductList : To get the list of all product. Parameters: int takeCount, int skipCount
2. GetProductDetail/{id}: To get the detail of a perticular product/item. Parameters: int ProductId
3. UpdateProduct: To update the details of the product. Parameters: UpdateProductRequest Modal
            e.g. {
                    "productId": 0,
                    "name": "string",
                    "description": "string",
                    "price": 0,
                    "category": 0
                  }
                  
                  -ProductId: integer type: Id of the product that the user wants to update.
                  - name: string type : Name of the product
                  - description: string type : description of the product
                  - price: decimal type: price of the product
                  - category: Category Enum Type: 1= Electronics,2= clothes
4. AddNewProduct: To add new product in the system. Parameters: AddNewProductRequest Modal 
        e.g.{
              "name": "string",
              "description": "string",
              "price": 0,
              "category": 0
            }
            - name: string type : Name of the product
            - description: string type : description of the product
            - price: decimal type: price of the product
            - category: Category Enum Type: 1= Electronics,2= clothes
5. DeleteProduct/{id}: delete the product. Parameters: int Id: product id that the user wants to delete.
