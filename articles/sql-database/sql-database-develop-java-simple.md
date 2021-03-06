---
title: Connect to SQL Database by using Java with JDBC on Windows | Microsoft Docs
description: Presents a Java code sample you can use to connect to Azure SQL Database. The sample uses JDBC, and it runs on a Windows client computer.
services: sql-database
documentationcenter: ''
author: LuisBosquez
manager: jhubbard
editor: genemi

ms.assetid: 08fc49b1-cd48-4dcc-a293-ff22a4d2d62c
ms.service: sql-database
ms.custom: development
ms.workload: drivers
ms.tgt_pltfrm: na
ms.devlang: java
ms.topic: article
ms.date: 02/03/2017
ms.author: lbosq

---
# Connect to SQL Database by using Java with JDBC on Windows
[!INCLUDE [sql-database-develop-includes-selector-language-platform-depth](../../includes/sql-database-develop-includes-selector-language-platform-depth.md)]

This topic presents a Java code sample that you can use to connect to Azure SQL Database. The Java sample relies on the Java Development Kit (JDK) version 1.8. The sample connects to an Azure SQL Database by using the JDBC driver.

## Step 1:  Configure Development Environment
[Configure development environment for Java development](https://docs.microsoft.com/sql/connect/jdbc/step-1-configure-development-environment-for-java-development/)

## Step 2: Create a SQL database
See the [getting started page](sql-database-get-started.md) to learn how to create a database.  

## Step 3: Get Connection String
[!INCLUDE [sql-database-include-connection-string-jdbc-20-portalshots](../../includes/sql-database-include-connection-string-jdbc-20-portalshots.md)]

> [!NOTE]
> If you are using the JTDS JDBC driver, then you will need to add "ssl=require" to the URL of the connection string and you need to set the following option for the JVM "-Djsse.enableCBCProtection=false". This JVM option disables a fix for a security vulnerability, so make sure you understand what risk is involved before setting this option.
> 
> 

## Step 4: Run sample code
* [Proof of concept connecting to SQL using Java](https://docs.microsoft.com/sql/connect/jdbc/step-3-proof-of-concept-connecting-to-sql-using-java/)

## Next steps
* Visit the [Java Developer Center](/develop/java/).
* Review the [SQL Database Development Overview](sql-database-develop-overview.md)
* More information on the [Microsoft JDBC Driver for SQL Server](https://docs.microsoft.com/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server/)

## Additional resources
* [Design Patterns for Multi-tenant SaaS Applications with Azure SQL Database](sql-database-design-patterns-multi-tenancy-saas-applications.md)
* Explore all the [capabilities of SQL Database](https://azure.microsoft.com/services/sql-database/)

