---
title: "Add model-driven app form navigation for related tables in Power Apps | MicrosoftDocs"
description: Learn how to add form navigation for related tables
ms.custom: ""
ms.date: 03/18/2020
ms.reviewer: ""

ms.suite: ""
ms.tgt_pltfrm: ""
ms.topic: "how-to"
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
  - "PowerApps"
author: "Mattp123"
ms.assetid: b4098c96-bce1-4f57-804f-8694e6254e81
caps.latest.revision: 15
ms.subservice: mda-maker
ms.author: "matp"
manager: "kvivek"
search.audienceType: 
  - maker
search.app: 
  - "PowerApps"
  - D365CE
---
# Add model-driven app form navigation for related tables

When an app user selects one of these links in a row, the associated view for the table is displayed. In this article, the form navigation pane is used to add links to related tables.
  
1. Sign in to [Power Apps](https://make.powerapps.com/?utm_source=padocs&utm_medium=linkinadoc&utm_campaign=referralsfromdoc).  
1. Expand **Data** in the left-hand menu and select **Tables**
1. Select the table you want, and then select the **Forms** area.
1. In the list, open a form with the type of **Main** to edit it.
1. Select **Switch to classic** to edit the form in the classic form designer.
  
1. To add a link to a related table, on **Home** tab, in the **Select** group, choose **Navigation**.  

    :::image type="content" source="media/form-navigation.png" alt-text="Show form navigation pane":::

     The **Relationship Explorer** pane displays on the right side of the form editor.  

1. In the **Relationship Explorer** pane, in the **Filter** list, select one of the following options:  
  
    - **Available Relationships**. Lists all the tables that can be related to the table the form is associated with.  
  
    - **1:N Relationships**. Lists tables that can be related in a 1:N relationship to the table the form is associated with.  
  
    - **N:N Relationships**. Lists tables that can be related in a N:N relationship to the table the form is associated with.  
  
    > [!NOTE]
    >  If no related tables show up in the **Relationship Explorer** pane, you cannot create a link on this form to a related table.  
  
2. Select the related table you want to link to, drag it to the Navigation Pane, and then drop it where you want it to be displayed.  
  
    > [!TIP]
    >  You can also create a new relationship by choosing **New 1:N** or **New N:N** in the **Relationship Explorer** pane.
  
3. To edit the properties for this or any other related table link, in the Navigation Pane, select the link, and then on the **Home** tab, choose **Change Properties**.  
4. In the **Relationship Properties** dialog, on the **Display** tab, type a new display label.  
5. On the **Name** tab, choose **Edit** to view or edit the details associated with the relationship row.  
6. Choose **OK**.
7. Preview how the main form will appear and how events will function:  
  
    1. On the **Home** tab, choose **Preview**, and then select **Create Form**, **Update Form**, or **Read-Only Form**.  
    2. To close the **Preview** form, on the **File** menu, choose **Close**.  
  
8. When you finish editing the form, choose **Save and Close** to close the form.  
9. When your customizations are complete, publish them:  
  
    - To publish customizations for only the component that you are currently editing, in the Navigation Pane, choose the table you have been working on, and then choose **Publish**.  
  
    - To publish customizations for all unpublished components at one time, in the Navigation Pane, choose **Tables**, and then on the command bar, choose **Publish All Customizations**.  
  
> [!NOTE]
> Installing a solution or publishing customizations can interfere with normal system operation. We recommend that you schedule a solution import when it's least disruptive to users.
  
## Next steps

 [Create and edit table relationships for Microsoft Dataverse](../data-platform/create-edit-entity-relationships.md)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
