---

copyright:
  years: 2016,2018
lastupdated: "2018-01-03"
---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# 定價
{: #pricing}

## 基本配置
{{site.data.keyword.composeForPostgreSQL_full}} 服務是具有兩個資料節點的叢集，每個資料節點包含 1GB 的儲存空間及 102MB 的記憶體，這等於 1 個資源單位。服務_包括_ 抄寫及高可用性，因此每個單位及單價_包括_ 這兩個節點中資源的成本。

基本配置也包括三個 etcd 仲裁程式膠囊（用來管理抄寫），以及兩個 HAProxy 膠囊（用於管理連線及失效接手）。HAProxy 膠囊每個都有 64MB 的記憶體。

### 成本
基本服務配置具有固定價格。請參閱 {{site.data.keyword.cloud_notm}} 上的型錄磚，以取得當地貨幣的基本定價。例如，以美元表示的基本價為 $12/月。

## 擴充選項
如果您的服務需要額外的儲存空間或記憶體，則可以使用磁碟儲存空間與記憶體單元的 10:1 比例來增加配置的資源。增加配置給部署的磁碟也會增加配置的 RAM。{{site.data.keyword.composeForPostgreSQL}} 單位由 1GB 的儲存空間與 102MB 的記憶體所組成，而且每個單位及單價_包括_ 在這兩個資料節點上增加資源的成本。

### 成本
每個額外單位（1GB 儲存空間/102MB 記憶體）都有單價，其會以當地貨幣列在服務的 {{site.data.keyword.cloud_notm}} 型錄磚上。以美元表示時，每個額外單位的成本為 $12。當您的所有 {{site.data.keyword.composeForPostgreSQL}} 服務的大小_總計_ 增加時，單價就會降低，如下面分級定價表所示。

### 分級定價
單位數|單價
----------|-----------
1 - 9 個單位|基本單價 -- $12.00 美元/單位
10 - 24 個單位|折價 10% --$10.80 美元/單位
25 - 49 個單位|折價 20% -- $9.60 美元/單位
50 - 99 個單位|折價 30% -- $8.40 美元/單位
100 - 499 個單位|折價 40% --$7.20 美元/單位
500 - 999 個單位|折價 50% -- $6.00 美元/單位
1,000 - 4,999 個單位|折價 60% -- $4.80 美元/單位
5,000 個以上單位|折價 70% -- $3.60 美元/單位
{: caption="表 1. {{site.data.keyword.composeForPostgreSQL}} 分級定價" caption-side="top"}