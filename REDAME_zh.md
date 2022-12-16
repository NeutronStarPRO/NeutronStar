# NeutronStar

**在 IC 上的 web3 Blog 内容聚合平台！**

> 分布式协作：为 NeutronStarDAO 贡献代码可以获得 token 奖励。


# 架构：

项目主要由 WeBlog 、NeutronStar、Seesset 部分组成。

* WeBlog 是一个独立的 blog 存储、发布工具
* NeutronStar 是 blog 内容聚合平台
* Seesset 是一个 NFT blog 交易平台

![3](assets/readme/3.png)

### WeBlog 独立存储：

作者的文章储存都在自己的 canister 里。 每个 WeBlog 用户可以创建一个自己的罐子用于存放自己的 blog 、图片。可以设置某篇 blog 公开，这样大家可以调作者的 canister 直接浏览 blog 。

### NeutronStar 社区 canister ：

作者还可以推送文章到社区 canister 让更多人看见。用户访问社区的 canister 来阅读文章。别的客户端也可以获取社区 canister 的内容。

社区的这些 canister 属于 NeutronStarDAO 。由 DAO 雇佣开发团队维护、升级 canister 。NSDAO 也负责审核、删除大家投票都不喜欢的内容（前期由团队托管 canister ，后面会成立 NSDAO ，然后交给 NSDAO）。

读者可以根据文章内容分类组成不同的兴趣小组、小社群交流讨论、一起投票等等。

### Seesset NFT:

作者写完 blog 后可以选择花费一些 NS 把 blog 铸造为 NFT 。

### 开放接口：

社区 canister 的接口是开放的。各种前端都可以连接到社区，而且其他类型的平台也可以向 NeutronStar 社区推送自己的文章，获取社区里的文章列表、文章内容，也可以通过这组开放接口完成交互：评论、点赞等等（但没有 NFT 文章系列功能）。

公共 API 输出的数据：

* 最新发表的文章的排名。

* 根据算法生成的热度排名，由浏览量、点赞数、评论数、评论数、评论点赞，共同决定（同时也决定了 NFT 文章的价格）。

* 某篇文章的具体内容、点赞、评论数据

<br/>


# 经济模型

Token 名称为 NS 。NS 总量为 100000000 枚。

* NS 用途：参与 NSDAO 投票、参与 NSDAO 治理、打赏作者、铸造 NFT blog

* NS 来源：发布文章并获得 NSDAO 认可、参与 blog 审核

作者可以直接发布普通 blog ，也可以选择把 blog 铸造成 NFT 发布（假设铸造 NFT 花了 10 NS ）。

当人们阅读 NFT blog 时，会获取一定数量的 NS ，先到先得，总共就会发放 2 NS（燃烧 80% NS ）， 晚几分钟可能就被领完了。 **奖励和比特币挖矿奖励机制类似，最开始阅读奖励最多，到后面按对数模型减少，直到 NS 发放完毕。** 

NFT blog 的浏览量、点赞数、评论数越多，NFT 的价格可能就越高，作者可以给 NFT 定价。

所有人都可以出价购买 NFT 来收藏，NSDAO 也会购买 NFT blog（**NSDAO 倾向于积极收藏各种精华 NFT blog ，为社区吸引更多读者、作者，正向循环。可能的一种情况是人们和 NSDAO 抢着收藏好 blog ，就像拍卖一样，由作者决定卖给谁了**）。

总之，如果作者觉得自己 blog 不错就买 NS 铸造 NFT blog，然后卖 NFT 赚钱；用户阅读 blog 获得 NS 。

如果作者没有铸造 NFT ，在 blog 发布后觉得自己的 blog 质量不错，也可以向 NSDAO 申请赞助。

<br/>

## 发起私人空间：

在社区里创建私人社区 canister 。

只有受创建者邀请才有（订阅）canister 访问权，空间里的所有人都能发文章，只有空间里的其他人能看见。也可以发 NFT blog 。canister 控制权归创建者。

<br/>

## 社区 NFT 徽章：

达成成就获得自己的专属徽章：第一次发表 blog 、第一次评论、文章阅读数超过 5000 ......

<br/>

---

作者还可以发起拍卖申请，社区投票，把人们一致认为优秀的 NFT blog 拍卖。



