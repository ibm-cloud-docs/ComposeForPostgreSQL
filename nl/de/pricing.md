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

# Preisstruktur
{: #pricing}

## Basiskonfiguration
Der {{site.data.keyword.composeForPostgreSQL_full}}-Service ist ein Cluster mit zwei Datenknoten mit jeweils 1 GB Speicher und 104 MB Hauptspeicher. Dies entspricht 1 Ressourceneinheit. Der Service _umfasst_ Replikation und Hochverfügbarkeit. In jedem Einzelpreis sind jeweils die Ressourcenkosten für beide Knoten _enthalten_.

Die Basiskonfiguration umfasst zudem drei etcd-Arbiter-Kapseln für die Verwaltung von Replikation und zwei HAProxy-Kapseln für die Verwaltung von Verbindungen und Failover. Jede HAProxy-Kapsel hat 64 MB Hauptspeicher.

### Kosten
Die Basisservicekonfiguration hat einen Festpreis. Den Grundpreis in Ihrer Landeswährung finden Sie über die entsprechenden Katalogkacheln auf {{site.data.keyword.cloud_notm}}. Der Grundpreis in US-Dollar beträgt zum Beispiel $12/Monat.

## Erweiterungsoptionen
Wenn Sie zusätzlichen Speicher oder Hauptspeicher für Ihren Service benötigen, können Sie die zugeordneten Ressourcen in einem Verhältnis von 10:1 von Plattenspeicher zu Speichereinheit erhöhen. Durch Erhöhen des der Bereitstellung zugeordneten Plattenspeichers erhöht sich der zugeordnete RAM entsprechend. Eine {{site.data.keyword.composeForPostgreSQL}}-Einheit besteht aus 1 GB Speicher und 102 MB Hauptspeicher. Im Einzelpreis pro Einheit sind die Kosten für die Erweiterung der Ressourcen auf beiden Datenknoten _enthalten_.

### Kosten
Jede zusätzliche Einheit (1 GB Speicher/102 MB Hauptspeicher) hat einen Einzelpreis, der auf der {{site.data.keyword.cloud_notm}}-Katalogkachel für den Service in Ihrer Landeswährung aufgelistet ist. In US-Dollar beträgt der Preis für jede zusätzliche Einheit $12. Mit zunehmender _Gesamtgröße_ Ihrer {{site.data.keyword.composeForPostgreSQL}}-Services verringert sich der Preis pro Einheit, wie aus der folgenden Tabelle zur gestaffelten Preisstruktur hervorgeht.

### Gestaffelte Preisstruktur
Anzahl der Einheiten|Einzelpreis
----------|-----------
1 - 9 Einheiten|Basiseinzelpreis -- $12,00 USD/Einheit
10 - 24 Einheiten|10% Ermäßigung -- $10,80 USD/Einheit
25 - 49 Einheiten|20% Ermäßigung -- $9,60 USD/USD/Einheit
50 - 99 Einheiten|30% Ermäßigung -- $8,40 USD/Einheit
100 - 499 Einheiten|40% Ermäßigung -- $7,20 USD/Einheit
500 - 999 Einheiten|50% Ermäßigung -- $6,00 USD/Einheit
1.000 - 4.999 Einheiten|60% Ermäßigung -- $4,80 USD/Einheit
5.000+ Einheiten|70% Ermäßigung -- $3,60 USD/Einheit
{: caption="Tabelle 1. Gestaffelte Preisstruktur von {{site.data.keyword.composeForPostgreSQL}}" caption-side="top"}