# 秒杀系统简介

##什么是秒杀活动
秒杀系统场景就是商品数量有限的情况，多个用户在秒杀活动开始后抢购商品的场景。
##例子：
某电商平台，预订了一个晚上8点整开始销售10件优惠力度很大的商品的活动，超过1万个用户，在活动开始前就在活动页面等待秒杀活动的开始，活动一开始，1万个用户在几秒之内就下单购买了产品。

##秒杀活动可能遇到的问题
    1.商品详情页面打不开，影响用户体验（页面打不开）和造成损失（商品没卖出去，或者超卖了），浏览量很大的问题
    2.有限的商品，可能会超卖，商品减库存的问题

##秒杀活动的问题根源
秒杀系统根本上问题，解释就是并发读，并发写。

##秒杀系统的关键
    1.稳，高可用
    2.准，一致性
    3.块，高性能

    