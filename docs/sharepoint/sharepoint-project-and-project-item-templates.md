---
title: "SharePoint Project and Project Item Templates | Microsoft Docs"
ms.custom: ""
ms.date: "02/22/2017"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "office-development"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "VS.SharePointTools.SPE.FirstWizardPage"
  - "VS.SharePointTools.SPE.ListInstance"
  - "VS.SharePointTools.SPE.ListDefinition"
  - "VS.SharePointTools.SPE.ListDefFromContentType"
  - "VS.SharePointTools.SPE.ContentType"
  - "SPE.Wizard"
dev_langs: 
  - "VB"
  - "CSharp"
  - "VB"
  - "CSharp"
helpviewer_keywords: 
  - "SharePoint development in Visual Studio, project and project item templates"
  - "SharePoint development in Visual Studio, templates"
ms.assetid: 54a7576f-d3f9-475d-8ed7-b675ad21cb53
caps.latest.revision: 41
author: "kempb"
ms.author: "kempb"
manager: "ghogen"
---
# SharePoint Project and Project Item Templates
  The following sections describe the available SharePoint project and project item templates and how they are used. 
  
##  Project and Project Item Templates Overview  
 When you create a new SharePoint project in Visual Studio, a SharePoint project is added to the solution together with all of the project items required by that project type. For example, if you create a Silverlight Web Part project, Visual Studio creates a solution that contains a Visual Web Part project item and a Silverlight application project item along with all the files required by those project items. Project item templates are used to add project items to an existing SharePoint project, such as adding an event receiver, site column, or list.  
  
 For information about SharePoint fundamentals, see [SharePoint Foundation Building Blocks](http://go.microsoft.com/fwlink/?LinkId=179404). Advanced users can create custom project and project item templates. For more information, see [Extending the SharePoint Project System](../sharepoint/extending-the-sharepoint-project-system.md).  
  
##  Project Templates  
 Following is a list of SharePoint project templates. To view the SharePoint project templates in Visual Studio, in the **New Project** dialog box, expand the **SharePoint** node under either **Visual C#** or **Visual Basic**, and then choose **2010**.  
  
### SharePoint 2010 Project  
 The contents of a *SharePoint 2010 Project* are included in every SharePoint project template. A SharePoint 2010 Project contains:  
  
-   A project file.  
  
-   A project properties page.  
  
-   A **References** folder listing all of the assembly references in the project.  
  
-   A **Features** folder that contains a .feature configuration file, used to deploy features to SharePoint server.  
  
-   A **Package** folder that contains a Package.package file, used to deploy the solution to SharePoint.  
  
-   A key.snk (strong-name key) file that is used to sign the assembly with a strong name, for enhanced security.  
  
### SharePoint 2010 Silverlight Web Part  
 *SharePoint 2010 Silverlight Web Part* projects enable you to create web parts for SharePoint that display Silverlight applications. When you create this project, you can specify whether to add a new Silverlight application to it or reference an existing one. For more information, see [Creating Web Parts for SharePoint](../sharepoint/creating-web-parts-for-sharepoint.md) and [Walkthrough: Creating a Silverlight Web Part that Displays OData for SharePoint](../sharepoint/walkthrough-creating-a-silverlight-web-part-that-displays-odata-for-sharepoint.md).  
  
### SharePoint 2010 Visual Web Part  
 A *SharePoint 2010 Visual Web Part* project includes an Elements.xml definition file, a **Web Part** item, and a **User Control** item. You can design the appearance of the visual web part by dragging or copying controls from the Visual Studio Toolbox to the surface of the user control. For more information, see [How to: Create a SharePoint Web Part by Using a Designer](../sharepoint/how-to-create-a-sharepoint-web-part-by-using-a-designer.md) and [Building Block: Web Parts](http://go.microsoft.com/fwlink/?LinkId=179438).  
  
### Import SharePoint 2010 Solution Package  
 *Import SharePoint 2010 Solution Package* projects let you import all or part of an existing SharePoint 2010 site, exported to a SharePoint solution (.wsp) file, into Visual Studio. Once imported into Visual Studio, you can customize its items and redeploy them. For more information, see [Importing Items from an Existing SharePoint Site](../sharepoint/importing-items-from-an-existing-sharepoint-site.md).  
  
### Import Reusable SharePoint 2010 Workflow  
 *Import Reusable SharePoint 2010 Workflow* projects let you import a reusable, declarative workflow created in SharePoint Designer 2010 into Visual Studio. The workflow is exported from the SharePoint site as a .wsp file. Once imported into Visual Studio, you can customize it, add code to it, and then deploy it to a SharePoint site. For more information, see [Walkthrough: Import a SharePoint Designer Reusable Workflow into Visual Studio](../sharepoint/walkthrough-import-a-sharepoint-designer-reusable-workflow-into-visual-studio.md).  
  
##  Project Item Templates  
 Following is a list of SharePoint project item templates. Project item templates add files to the SharePoint solution to support SharePoint functionality such as site columns, lists, and content types. For example, adding a site column to your solution adds a site column project that contains an Elements.xml definition file. Adding a visual web part adds a visual web part project to your solution that contains an Elements.xml file, a user control item, and a visual web part item.  
  
 To view the SharePoint project item templates, in **Solution Explorer**, open the shortcut menu for a SharePoint project, and then choose **Add**, **New Item**. Expand the **SharePoint** node under either **Visual C#** or **Visual Basic**, and then choose **2010**.  
  
### Application Page (Farm Solution Only)  
 An **Application Page (Farm Solution Only)** item enables you to design an [!INCLUDE[vstecasp](../sharepoint/includes/vstecasp-md.md)] web page for a SharePoint site. Applications pages can be used only in farm solutions. You can add this project item only to farm solutions. For more information, see [How to: Create an Application Page](../sharepoint/how-to-create-an-application-page.md) and [Application _layouts Page Type](http://go.microsoft.com/fwlink/?LinkId=179434).  
  
### Business Data Connectivity Model (Farm Solution Only)  
 A **Business Data Connectivity Model (Farm Solution Only)** item enables you to integrate business data into SharePoint. Business data can come from back-end server applications, such as [!INCLUDE[ssNoVersion](../sharepoint/includes/ssnoversion-md.md)], Siebel, and Service Advertising Protocol (SAP). Business data connectivity models can be used only in farm solutions. You can add this project item only to farm solutions. For more information, see [How to: Create a BDC Model](../sharepoint/how-to-create-a-bdc-model.md), [How to: Use a Resource File to Specify Localized Names, Properties, and Permissions](../sharepoint/how-to-use-a-resource-file-to-specify-localized-names-properties-and-permissions.md), and [What's New: Business Connectivity Services](http://go.microsoft.com/fwlink/?LinkId=179411).  
  
### Content Type  
 *Content Type* items let you create custom content types based on an existing (base) content type such as a document, announcement, or a task. A custom content type provides the same attributes and fields as the base content type together with any site columns (fields) you define. For example, you can create a custom Contact content type that is based on the base Contact content type that comes in SharePoint. You can customize the content type by changing the existing site columns or adding more site columns to the ones already included in the base content type.  
  
> [!NOTE]  
>  Due to a SharePoint limitation, you cannot create a farm solution content type based on a sandboxed solution content type.  
  
 For more information, see [Walkthrough: Create a Site Column, Content Type, and List for SharePoint](../sharepoint/walkthrough-create-a-site-column-content-type-and-list-for-sharepoint.md) and [Building Block: Content Type](http://go.microsoft.com/fwlink/?LinkId=179413).  
  
### Empty Element  
 *Empty elements* are most often used to define SharePoint project items that lack a project or project item template in Visual Studio. When you add an empty element to your project, a node named EmptyElement[x](where [x] is a unique number\) is created. EmptyElement[x] contains a single file that is named Elements.xml. Use [!INCLUDE[TLA2#tla_xml](../sharepoint/includes/tla2sharptla-xml-md.md)] statements to define the desired elements in Elements.xml.  
  
### Event Receiver  
 *Event receivers* handle events for items in the SharePoint site, such as when an item is added to a list, when a web item is deleted, or when a workflow started. The event receiver project item template lets you handle  
  
-   List events  
  
-   List item events  
  
-   List email events  
  
-   Web events  
  
-   List workflow events  
  
 The event receiver project item creates an **Event Receiver** folder with a single class file that contains event handlers for all of the events you specified when you created the project in the **SharePoint Customization Wizard**. The event receiver class can handle events that occur on the SharePoint site when items such as files, fields, items, lists, attachments, web parts, and workflows are added, updated, deleted, or removed. For more information, see [How to: Create an Event Receiver](../sharepoint/how-to-create-an-event-receiver.md) and [Building Block: Event Handling](http://go.microsoft.com/fwlink/?LinkId=179416).  
  
### List  
 A list is an instance of a reusable base SharePoint list definition, such as a calendar or a task list. After adding a list to your solution, the List Designer enables you to add site columns to the list and create custom list columns. This includes site columns from content types. You can specify the *view* for the list, which determines the columns that will appear in the list. For more information, see [Walkthrough: Create a Site Column, Content Type, and List for SharePoint](../sharepoint/walkthrough-create-a-site-column-content-type-and-list-for-sharepoint.md) and [Building Block: Lists and Document Libraries](http://go.microsoft.com/fwlink/?LinkId=179421).  
  
### Module  
 *Modules* (not to be confused with [!INCLUDE[vbprvb](../sharepoint/includes/vbprvb-md.md)] modules) contain any files that you want to deploy to the SharePoint server, such as images or notes. The module project item contains a **Module** node. The module node contains two project item templates: an XML definition file, which acts as a manifest for the module, and a sample.txt file, a placeholder file. For more information, see [Using Modules to Include Files in the Solution](../sharepoint/using-modules-to-include-files-in-the-solution.md) and [Modules](http://go.microsoft.com/fwlink/?LinkId=179425).  
  
### Sequential Workflow (Farm Solution Only)  
 A *sequential workflow* is a series of business logic steps, performed in sequence, until the last step is completed. Sequential workflows are used to manage processes that involve SharePoint items such as lists and documents. You can create either site-level (global) workflows or list-level (local) workflows, and you can select whether a workflow starts automatically or manually. This project item can be used only in farm solutions. You can add this project item only to farm solutions. For more information, see [Creating SharePoint Workflow Solutions](../sharepoint/creating-sharepoint-workflow-solutions.md), [Workflows in SharePoint Server 2010](http://go.microsoft.com/fwlink/?LinkId=260555), and [What's New: Workflow Improvements](http://go.microsoft.com/fwlink/?LinkId=179418).  
  
### Silverlight Web Part  
 *Silverlight web part* project items enable you to create web parts for SharePoint that display Silverlight applications. When you add this project item to your solution, you can choose whether to add a new Silverlight application or reference an existing one later. For more information, see [Creating Web Parts for SharePoint](../sharepoint/creating-web-parts-for-sharepoint.md) and [Walkthrough: Creating a Silverlight Web Part that Displays OData for SharePoint](../sharepoint/walkthrough-creating-a-silverlight-web-part-that-displays-odata-for-sharepoint.md).  
  
### Site Column  
 A *site column*, also known as a *field*, is one of the most basic elements you can add to a SharePoint project. A site column represents a type of data, such as a telephone number, a text comment, or the city name of a contact in a contact list. For more information, see [Creating Site Columns, Content Types, and Lists for SharePoint](../sharepoint/creating-site-columns-content-types-and-lists-for-sharepoint.md) and [Columns](http://go.microsoft.com/fwlink/?LinkId=226840).  
  
### Site Definition (Farm Solution Only)  
 *Site definition* project items contain a site definition folder that includes the following files:  
  
-   A default .aspx page, used as the default web page for the site.  
  
-   An onet.xml file that defines the components of the site.  
  
-   A webtemp xml file that specifies the site definition configurations that appear in the **Template Selection** section of the **New SharePoint Site** page.  
  
 After you add a site definition, you add code and files to introduce functionality. This project item can be used only in farm solutions. You can add this project item only to farm solutions. For more information, see [Creating Site Definitions for SharePoint](../sharepoint/creating-site-definitions-for-sharepoint.md) and [Site Definitions and Configurations](http://go.microsoft.com/fwlink/?LinkId=260554).  
  
### State Machine Workflow (Farm Solution Only)  
 A *state machine workflow* is a set of business logic states, transitions, and actions. The steps in a state machine workflow are not performed in sequence; instead, they are triggered by actions and states. Like a sequential workflow, state machine workflows are associated with SharePoint items such as lists and documents. Once again, you can create site-level (global) workflows or list-level (local) workflows. You can also select whether a workflow starts automatically or manually. This project item can be used only in farm solutions. You can add this project item only to farm solutions. For more information, see [Creating SharePoint Workflow Solutions](../sharepoint/creating-sharepoint-workflow-solutions.md), [Workflows in SharePoint Server 2010](http://go.microsoft.com/fwlink/?LinkId=260555),  and [What's New: Workflow Improvements](http://go.microsoft.com/fwlink/?LinkId=179418).  
  
### User Control (Farm Solution Only)  
 A *user control* is a custom, reusable control to which you can add other ASP.NET controls and SharePoint controls. The user control can be added to application pages and web parts that run in SharePoint. This project item can be used only in farm solutions. You can add this project item only to farm solutions. For more information, see [Creating Reusable Controls for Web Parts or Application Pages](http://go.microsoft.com/fwlink/?LinkId=226841).  
  
### Visual Web Part  
 A *visual web part* project item includes an Elements.xml definition file, a **Web Part** item, and a **User Control** item. You can design the appearance of the visual web part by dragging or copying controls from the Visual Studio Toolbox to the surface of the user control. For more information, see [How to: Create a SharePoint Web Part by Using a Designer](../sharepoint/how-to-create-a-sharepoint-web-part-by-using-a-designer.md) and [Building Block: Web Parts](http://go.microsoft.com/fwlink/?LinkId=179438).  
  
### Web Part  
 A *web part* is a server-side control that runs inside a special type of page called a Web Part Page. They are the building blocks of pages that appear on a SharePoint site. The web part item provides files that enable you to design a web part for a SharePoint site. For more information, see [How to: Create a SharePoint Web Part](../sharepoint/how-to-create-a-sharepoint-web-part.md) and [Building Block: Web Parts](http://go.microsoft.com/fwlink/?LinkId=179438).  
  
## See Also  
 [Developing SharePoint Solutions](../sharepoint/developing-sharepoint-solutions.md)   
 [SharePoint Products and Technologies](http://go.microsoft.com/fwlink/?LinkId=178818)  
  
  