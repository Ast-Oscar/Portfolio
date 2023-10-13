---
title: Order Manager in SQL and C# 
publishDate: 2023-05-25 00:00:00
img: ../../assets/bdd_miniature.jpg
img_alt: Our E/A schema
description: |
  In my third year, we created a database in SQL that could be updated through a Windows Forms linked to a C# program
tags:
  - SQL
  - MySQL
  - C#
  - Windows Forms
  - ASP.NET
  - XML
---

<p style="width: 100%">
  
  ## Creating the system
  We were able to create the database on **MySQL Workbench** with the help of the relational schema. 
</p>

<img src="../../assets/Schema_ea.jpg" alt="our relational entity-attributes schema" width="100%">
<p style="width: 100%">  
  The insertion of values was however difficult given the configuration of the database at the order type level. We have filled our database by hand, then we completed it once the **C#** code operational. It was much more convenient and comfortable. 
  
  We decided to use a **WebApplication Framework** for the graphical interface of the information system of Mr. Bellefleur (the given name of the salesman manager) and for the interface of customers. We therefore use **ASP.NET** **WebForms** to give the overall structure of each page and to integrate the C# code behind.
  
  ## Demonstration
</p>

<video controls width="100%" muted controlsList="nodownload">
  <source src="../../assets/bellefleur_demo.mp4" type="video/mp4">
</video>
