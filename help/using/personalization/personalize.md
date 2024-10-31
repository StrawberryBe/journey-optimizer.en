---
solution: Journey Optimizer
product: journey optimizer
title: Personalize content in Journey Optimizer
description: Get Started with personalization.
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
keywords: expression, editor, start, personalization
exl-id: f448780b-91bc-455e-bf10-9a9aee0a0b24
---
# Get started with personalization{#add-personalization}

>[!CONTEXTUALHELP]
>id="ajo_homepage_card5"
>title="Personalize experiences"
>abstract="Use **Adobe Journey Optimizer** to adapt your messages to each specific recipient by leveraging the data and information you have about them. It can be their first name, interests, where they live, what they bought, and more."

Discover [!DNL Adobe Journey Optimizer] personalization capabilities to adapt your messages to each specific recipient by leveraging the data and information you have about them. It can be their first name, interests, where they live, what they bought, and more.  

➡️ [Learn how to personalize a message in these videos](#video-perso)
➡️ [Discover use cases leveraging personalization](personalization-use-case.md)

## Build personalization expressions using a dedicated syntax {#syntax}

[!DNL Journey Optimizer] uses an **inline** simple personalization syntax based on Handlebars which allows you to create expressions with contents enclosed by double curly braces **{{}}**. You can add multiple expressions in the same content or field without restrictions. Learn more in [Personalization syntax](personalization-syntax.md).

**Examples:**

* `Hello {{profile.person.name.firstName}} {{profile.person.name.lastName}}`
* `Hello {{profile.person.name.fullName}}`

When processing the message (email and push), Journey Optimizer replaces the expression with the data contained in the Experience Platform database:  `Hello {{profile.person.name.firstName}} {{profile.person.name.lastName}}` becomes "Hello John Doe".

## Leverage profile data to personalize your messages {#data}

The personalization is based on the profile data that are managed by the **XDM Individual Profile** schema defined in Adobe Experience Platform. Learn more in [Adobe Experience Platform Data Model (XDM) documentation](https://experienceleague.adobe.com/docs/experience-platform/xdm/home.html){target="_blank"}.

>[!CAUTION]
>The **XDM Individual Profile** schema is the only schema you can use to personalize content in [!DNL Journey Optimizer].

In addition, you can also leverage **computed attributes** to personalize your content. Computed attributes are based on Profile-enabled Experience Event datasets ingested into Adobe Experience Platform and serve as aggregated data points stored within customer profiles that summarize individual behavioral events [Learn how to work with computed attributes](../audience/computed-attributes.md)

## Add personalization in different contexts {#contexts}

[!DNL Journey Optimizer] allows you to personalize the content and display of messages in several different ways. Learn more about the contexts where you can perform personalization in [this section](personalization-contexts.md).

## Work with the expression editor {#editor}

[!DNL Journey Optimizer] provides an expression editor where you will select, arrange, customize and validate all the data to create a customized personalization for your content.

Several tools are available to help build your personalization content, such as: helper functions, pre-defined expressions library, attributes favouriting, and more.

Learn more about [!DNL Journey Optimizer] expression editor in [this section](personalization-build-expressions.md)

## How-to videos{#video-perso}

Learn how to use contextual event information from a journey to personalize a message.

>[!VIDEO](https://video.tv.adobe.com/v/334165?quality=12)

Learn how to add profile-based personalization to a message and how to use audience membership as a pre-condition to a personalization block.

>[!VIDEO](https://video.tv.adobe.com/v/334078?quality=12)
 
