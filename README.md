# Katachii-overview

유리공예 작가 Nara님의 심플한 개인 쇼핑몰.

약 100명의 회원이 작가님의 작품을 구매하기 위해 이용하고 있습니다.

1인 개발자로서 ‘기획, 프론트엔드, 백엔드, 배포’ 전과정을 담당하여 개발하였습니다.

-----

## Overview.

> 서비스 미리보기
> 

### Mobile:

[<img src="https://img.youtube.com/vi/23tY3lR6LMs/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/23tY3lR6LMs)

### PC:

[<img src="https://img.youtube.com/vi/e49wtjRZMfs/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/e49wtjRZMfs)

<br/>

## Key Features.

- **회원가입 & 로그인**
    
[<img src="https://img.youtube.com/vi/ZUm74YLlPYg/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/ZUm74YLlPYg)

- **상품 상세 페이지 & 장바구니(cart)**
    
[<img src="https://img.youtube.com/vi/E9k46ehkUfw/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/E9k46ehkUfw)

- **상품 구매**
    
[<img src="https://img.youtube.com/vi/zEoGBrzy0pc/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/zEoGBrzy0pc)

- **마이페이지**
    
[<img src="https://img.youtube.com/vi/g6Z6DobrOVA/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/g6Z6DobrOVA)

<br/>

-----

## 개선사항

- 

### [FE] 사용자들에게 좀더 직관적인 UI/UX 적용

- Version 01에서는:
    
[<img src="https://img.youtube.com/vi/pdMzjuVnB4E/hqdefault.jpg" width="600" height="300"
/>](https://www.youtube.com/embed/pdMzjuVnB4E)

- **상세설명:**
    - **랜딩 페이지:**
        - [ 버전 1 ] - 버전1에서는 유저가 처음 랜딩페이지에 진입했을 때, 상품 리스트를 보기 위해 아래로 스크롤을 내려야 했습니다. 이는 직관적이지 않아 많은 유저들에게 혼란을 주었습니다.
          
            <img width="238" alt="스크린샷 2023-07-31 오후 12 00 20" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/614cc143-9813-4f8f-a7a0-ae7d5a522a9b">

            
        - [ 버전 2 ] - 햄버거 메뉴와 사이드바를 도입해 좀더 친숙하고 직관적인 랜딩 페이지를 제공하였습니다.
            
            <img width="311" alt="스크린샷 2023-07-31 오후 12 00 53" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/66c823e4-5b56-4021-93c1-4df20a051bdb">
            
    - **상품 상세 페이지:**
        - [ Version 1 ] - users had to scroll all the way down to the bottom in the product details page in order to find the CTA button for adding to cart or proceeding to purchase.
            
          <img width="239" alt="스크린샷 2023-07-31 오후 12 03 20" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/8b48b794-51c3-4df3-b2b6-a597d56cde5d">

            
        - [ Version 2 ] - After finding out that the majority of users to our service were using mobile, I had the CTA buttons stick on the bottom of the screen all the time in product details page and added bottom sheet for mobile to easily add to cart or proceed to purchase.
     
            <img width="144" alt="스크린샷 2023-07-31 오후 12 04 26" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/786bcb41-baa5-4cf2-a493-45c905dd4bf2">
            
    
    - **Purchase Page:**
        - [ Version 1 ]
            
          
          <img width="240" alt="스크린샷 2023-07-31 오후 12 06 36" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/fe1b3110-6a4b-416b-8c28-c4455af5c438">

        - [ Version 2 ] - By dividing the overall payment process into 'Customer Information,' 'Order Details,' and 'Payment,' users can now complete their orders more conveniently and intuitively.

          <img width="106" alt="스크린샷 2023-07-31 오후 12 07 17" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/a42f3cfb-f712-4315-a1f8-edd98475dec2">
            
    
    - **My Page:**
        - [ Version 1 ] - there weren’t many functionalities in my page previously. Users could only see the list of their orders and brief indicators for delivery status.
            
            <img width="332" alt="스크린샷 2023-07-31 오후 12 07 57" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/cd0764a0-f9bc-4ffd-971b-d25dedfcfdc1">

        - [ Version 2 ] - now the users can do a lot more in their my page.
            - 1) Users can change their password.
            - 2) Users can save up to 3 addresses so that they can simply choose from the address list during the purchase process instead of having to fill it out all over again every time they place an order.
            - 3) Users can now see the orders they have made with greater clarity.
                 
            <img width="119" alt="스크린샷 2023-07-31 오후 12 08 22" src="https://github.com/Alice-Yoon/Version-2.-Katachii/assets/53468065/984a4f9a-ddaa-4832-a457-a7829b27a8e9">
            

### [BE] Improved code maintainability by..

1) Applying Restful API

- open to see the code
    
    ```jsx
    // Ver 01:
    GET /api/products/getProducts
    GET /api/products/product_by_id?id={productId}
    POST /api/products/uploadProduct
    DELETE /api/products/deleteProduct
    
    // Ver 02:
    GET /api/v1/products
    GET /api/v1/products/:id
    POST /api/v1/products
    PUT /api/v1/products/:id
    DELETE /api/v1/products/:id
    ```
    

2) Separating routes and controllers

- open to see the code
    
    ```jsx
    ///////////////////
    ///// Ver 01: /////
    ///////////////////
    router.get('/getProducts', async (req, res) => {
        try {
            const products = await Product.find().exec();
            if(!products) return res.status(400).json({ success:  false, msg: '상품목록을 찾지 못했습니다.'});
    
            res.status(200).json({ success: true, products });
        } catch (err) {
            res.status(400).json({ success: false, err })
        }
    })
    
    ///////////////////
    ///// Ver 02: /////
    ///////////////////
    
    // - Getting products list
    router
      .route('/')
      .get(getProducts)
    
    exports.getProducts = async (req, res, next) => {
      res.status(200).json(res.advancedResults)
    };
    
    // - Getting single product info
    router
      .route('/:id')
      .get(getProduct)
    
    exports.getProduct = async (req, res, next) => {
    	const product = await Product.findById(req.params.id).populate(category);
    
    	if(!product) {
        return next(
    				new ErrorResponse(`No product found with id of ${req.params.id}`, 
    				404
    		);
      }
    
      res.status(200).json({
        success: true,
        data: product
      })
    }
    ```
    

### [BE] Increased code reusability and eliminated duplicate code by implementing middlewares.

- open to see the code
    
    ```jsx
    // Ver 02:
    
    /////////////////////
    //// Middleware /////
    /////////////////////
    const advancedResults = (
      model, 
      populateList = [], 
      searchQueryList = [],
      sort = {createdAt: -1}
    ) => async (req, res, next) => {
    
      // Generate SearchQuery
      const searchQuery = {}
      if(searchQueryList.length) {
        searchQueryList.forEach(searchQueryKey => {
          if(req.query[searchQueryKey]) {
            searchQuery[searchQueryKey] = req.query[searchQueryKey]
          }
        })
      }
    
      // Pagination
      const page = parseInt(req.query.page) || 1;
      const limit = parseInt(req.query.limit) || 10;
      const startIndex = (page - 1) * limit;
      const endIndex = page * limit;
      const total = await model.countDocuments(searchQuery);
      const totalPages = Math.ceil(total/limit);
    
      const pagination = {};
    
      if(endIndex < total) {
        pagination.next = {
          page: page + 1,
          limit
        }
      }
    
      if(startIndex > 0) {
        pagination.prev = {
          page: page - 1,
          limit
        }
      }
    
      const query = model.find(searchQuery);
      
      // Populate
      if(populateList.length) {
        populateList.forEach(pop => {
          query.populate(pop)
        })
      } 
    
      const totalDocumentCount = await model.countDocuments();
    
      const results = await query.sort(sort).skip(startIndex).limit(limit);
    
      res.advancedResults = {
        success: true,
        count: results.length,
        totalDocumentCount,
        totalPages,
        pagination,
        data: results
      }
    
      next(); 
    }
    
    //////////////////
    ///// Routes /////
    //////////////////
    
    // - Products list
    router
      .route('/')
      .get(
        advancedResults(
          Product, 
          [ // populate list
            { path: 'makeType', select: 'title' },
            { path: 'productType', select: 'title' },
            { path: 'category', select: 'title' },
          ], 
          [ // searchQuery list
            'isSoldOut',
            'makeType',
            'productType',
            'category'
          ], // sort
          { isSoldOut: 1, createdAt: -1 }
        ),
        getProducts
    )
    
    // - Orders list
    router
        .route('/orders')
        .get(
            protect,
            authorize('admin'),
            advancedResults(
                Order,
                [ // populate list
                    { path: 'products.productInfo.id', model: 'Product', select: 'thumbnail' },
                    { path: 'user', model: 'User', select: 'name' }
                ],
                [ // searchQuery list
                    'paymentStatus',
                    'deliveryStatus'
                ]
            ),
            getOrders
    )
    
    // - Users list
    router
      .route('/')
      .get(
        protect, authorize('admin'),
        advancedResults(
          User,
          [ // populate list
            { path: 'orders', select: '_id' }
          ],
          [ // searchQuery list
            'status'
          ]
        ),
        getUsers
      )
    ```
    

<br/>

