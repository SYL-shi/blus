classDiagram
    class AdminUser {
        - adminUserId: int
        - loginUserName: String
        - loginPassword: String
        - locked: int
        + AdminUser()
        + getAdminUserId(): int
        + setAdminUserId(adminUserId: int): void
        + getLoginUserName(): String
        + setLoginUserName(loginUserName: String): void
        + getLoginPassword(): String
        + setLoginPassword(loginPassword: String): void
        + getLocked(): int
        + setLocked(locked: int): void
    }

    class GoodsCategory {
        - categoryId: long
        - categoryLevel: int
        - parentId: long
        - categoryName: String
        - categoryRank: int
        - isDeleted: int
        - createTime: Date
        - createUser: int
        - updateTime: Date
        - updateUser: int
        + GoodsCategory()
        + getCategoryId(): long
        + setCategoryId(categoryId: long): void
        + getCategoryLevel(): int
        + setCategoryLevel(categoryLevel: int): void
        + getParentId(): long
        + setParentId(parentId: long): void
        + getCategoryName(): String
        + setCategoryName(categoryName: String): void
        + getCategoryRank(): int
        + setCategoryRank(categoryRank: int): void
        + getIsDeleted(): int
        + setIsDeleted(isDeleted: int): void
        + getCreateTime(): Date
        + setCreateTime(createTime: Date): void
        + getCreateUser(): int
        + setCreateUser(createUser: int): void
        + getUpdateTime(): Date
        + setUpdateTime(updateTime: Date): void
        + getUpdateUser(): int
        + setUpdateUser(updateUser: int): void
    }

    class GoodsInfo {
        - goodsId: long
        - goodsName: String
        - goodsIntro: String
        - goodsCategoryId: long
        - goodsCoverImg: String
        - goodsCarousel: String
        - goodsDetailContent: String
        - originalPrice: int
        - sellingPrice: int
        - stockNum: int
        - tag: String
        - goodsSellStatus: int
        - createUser: int
        - createTime: Date
        - updateUser: int
        - updateTime: Date
        + GoodsInfo()
        + getGoodsId(): long
        + setGoodsId(goodsId: long): void
        + getGoodsName(): String
        + setGoodsName(goodsName: String): void
        + getGoodsIntro(): String
        + setGoodsIntro(goodsIntro: String): void
        + getGoodsCategoryId(): long
        + setGoodsCategoryId(goodsCategoryId: long): void
        + getGoodsCoverImg(): String
        + setGoodsCoverImg(goodsCoverImg: String): void
        + getGoodsCarousel(): String
        + setGoodsCarousel(goodsCarousel: String): void
        + getGoodsDetailContent(): String
        + setGoodsDetailContent(goodsDetailContent: String): void
        + getOriginalPrice(): int
        + setOriginalPrice(originalPrice: int): void
        + getSellingPrice(): int
        + setSellingPrice(sellingPrice: int): void
        + getStockNum(): int
        + setStockNum(stockNum: int): void
        + getTag(): String
        + setTag(tag: String): void
        + getGoodsSellStatus(): int
        + setGoodsSellStatus(goodsSellStatus: int): void
        + getCreateUser(): int
        + setCreateUser(createUser: int): void
        + getCreateTime(): Date
        + setCreateTime(createTime: Date): void
        + getUpdateUser(): int
        + setUpdateUser(updateUser: int): void
        + getUpdateTime(): Date
        + setUpdateTime(updateTime: Date): void
    }

    class IndexConfig {
        - configId: long
        - configName: String
        - configType: int
        - goodsId: long
        - redirectUrl: String
        - configRank: int
        - isDeleted: int
        - createTime: Date
        - createUser: int
        - updateTime: Date
        - updateUser: int
        + IndexConfig()
        + getConfigId(): long
        + setConfigId(configId: long): void
        + getConfigName(): String
        + setConfigName(configName: String): void
        + getConfigType(): int
        + setConfigType(configType: int): void
        + getGoodsId(): long
        + setGoodsId(goodsId: long): void
        + getRedirectUrl(): String
        + setRedirectUrl(redirectUrl: String): void
        + getConfigRank(): int
        + setConfigRank(configRank: int): void
        + getIsDeleted(): int
        + setIsDeleted(isDeleted: int): void
        + getCreateTime(): Date
        + setCreateTime(createTime: Date): void
        + getCreateUser(): int
        + setCreateUser(createUser: int): void
        + getUpdateTime(): Date
        + setUpdateTime(updateTime: Date): void
        + getUpdateUser(): int
        + setUpdateUser(updateUser: int): void
    }

    class Order {
        - orderId: long
        - orderNo: String
        - userId: long
        - totalPrice: int
        - payStatus: int
        - payType: int
        - payTime: Date
        - orderStatus: int
        - extraInfo: String
        - userName: String
        - userPhone: String
        - userAddress: String
        - isDeleted: int
        - createTime: Date
        - updateTime: Date
        + Order()
        + getOrderId(): long
        + setOrderId(orderId: long): void
        + getOrderNo(): String
        + setOrderNo(orderNo: String): void
        + getUserId(): long
        + setUserId(userId: long): void
        + getTotalPrice(): int
        + setTotalPrice(totalPrice: int): void
        + getPayStatus(): int
        + setPayStatus(payStatus: int): void
        + getPayType(): int
        + setPayType(payType: int): void
        + getPayTime(): Date
        + setPayTime(payTime: Date): void
        + getOrderStatus(): int
        + setOrderStatus(orderStatus: int): void
        + getExtraInfo(): String
        + setExtraInfo(extraInfo: String): void
        + getUserName(): String
        + setUserName(userName: String): void
        + getUserPhone(): String
        + setUserPhone(userPhone: String): void
        + getUserAddress(): String
        + setUserAddress(userAddress: String): void
        + getIsDeleted(): int
        + setIsDeleted(isDeleted: int): void
        + getCreateTime(): Date
        + setCreateTime(createTime: Date): void
        + getUpdateTime(): Date
        + setUpdateTime(updateTime: Date): void
    }

    class OrderItem {
        - orderItemId: long
        - orderId: long
        - goodsId: long
        - goodsName: String
        - goodsCoverImg: String
        - sellingPrice: int
        - goodsCount: int
        - createTime: Date
        + OrderItem()
        + getOrderItemId(): long
        + setOrderItemId(orderItemId: long): void
        + getOrderId(): long
        + setOrderId(orderId: long): void
        + getGoodsId(): long
        + setGoodsId(goodsId: long): void
        + getGoodsName(): String
        + setGoodsName(goodsName: String): void
        + getGoodsCoverImg(): String
        + setGoodsCoverImg(goodsCoverImg: String): void
        + getSellingPrice(): int
        + setSellingPrice(sellingPrice: int): void
        + getGoodsCount(): int
        + setGoodsCount(goodsCount: int): void
        + getCreateTime(): Date
        + setCreateTime(createTime: Date): void
    }

    class ShoppingCartItem {
        - cartItemId: long
        - userId: long
        - goodsId: long
        - goodsCount: int
        - isDeleted: int
        - createTime: Date
        - updateTime: Date
        + ShoppingCartItem()
        + getCartItemId(): long
        + setCartItemId(cartItemId: long): void
        + getUserId(): long
        + setUserId(userId: long): void
        + getGoodsId(): long
        + setGoodsId(goodsId: long): void
        + getGoodsCount(): int
        + setGoodsCount(goodsCount: int): void
        + getIsDeleted(): int
        + setIsDeleted(isDeleted: int): void
        + getCreateTime(): Date
        + setCreateTime(createTime: Date): void
        + getUpdateTime(): Date
        + setUpdateTime(updateTime: Date): void
    }

    class User {
        - userId: long
        - name: String
        - password: String
        - address: String
        - isDeleted: int
        - lockedFlag: int
        - createTime: Date
        + User()
        + getUserId(): long
        + setUserId(userId: long): void
        + getName(): String
        + setName(name: String): void
        + getPassword(): String
        + setPassword(password: String): void
        + getAddress(): String
        + setAddress(address: String): void
        + getIsDeleted(): int
        + setIsDeleted(isDeleted: int): void
        + getLockedFlag(): int
        + setLockedFlag(lockedFlag: int): void
        + getCreateTime(): Date
        + setCreateTime(createTime: Date): void
    }

    User "1" -- "*" ShoppingCartItem : has
    User "1" -- "*" Order : places
    Order "1" -- "*" OrderItem : contains
    GoodsCategory "1" -- "*" GoodsInfo : categorizes
    IndexConfig "1" -- "*" GoodsInfo : configures
    GoodsInfo "1" -- "*" ShoppingCartItem : in
    GoodsInfo "1" -- "*" OrderItem : in
