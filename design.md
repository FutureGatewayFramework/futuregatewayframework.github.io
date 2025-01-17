---
layout: default
title: Design
permalink: /design/
order: 3
---

# Design Principles
Many of the ideas behind the FGF have been extracted from the:

|**Definition** [[XEDE](https://www.xsede.org/ecosystem/science-gateways)]|
|---|
|*A **Science Gateway** is a community-developed set of tools, applications, and data that is integrated via a portal or a suite of applications, usually in a graphical user interface, that is further customized to meet the needs of a specific community.*|

In particular, the following **keywords** used int the definition have been used as source of inspiration:

|---|
|**Communities**|SGs are targeted to serve one or many communities. The FGF handles user membership, provides groups and different level of authorisation.|
|**Tools, applications and data** integration|SGs are made of different components operating at different levels, the FGF provides API, libraries and tools ranging from the computing system back-end up to the user front-end.|
|**GUIs**|SGs can offer many kind of user level front-ends such as Web, desktop and mobile applications. FGF APIs, tools and libraries are capable to cope all these kind of user interfaces.|
|**Customization**|Serverd communities often require their own specific customisations that SGs should easily provide. The FGF structure has been specifically thought to allow any kind of customisation.|

# Key features
Beside keyords above, the FGF has the following key features:

|**KF1**|**Ease the installation and the maintenance**|
|---|---|
||• FGF provides installation and maintenance scripts. Officially the FGF components foresees the installation on top of an Ubuntu >= 16.04, however setup scripts have been structured in a way that the installation process can be migrated to other platforms. For instance the MacOS installation set demonstrates this capability just exploting the [`brew`][BREW] package management tool.|
||• All FGF components are available on [GitHub][GITHUB] and their source code licenced under the [Apache2][APACHE2] terms. |
||• Customizable for different community needs. Adopters may use official releases or extract FGF from its master branch or even work on a forked version allowing any kind of customisation.|

|**KF2**|**Flexible and structured access to DCIs through the use of pluggable components**|
|---|---|
||• Potentially the FGF can access any kind of DCI using pluggable components called **executor interfaces**. FGF provides its own standard executor interfaces: Grid and [Cloud Engine][G&CENG] ([JSAGA][JSAGA]) and [Tosca][TOSCAORCH] ([INDIGO-dc][INDIGODC] PaaS orchestrator).|
||• Advanced users may integrate new DCIs without affecting the SG front-end, moreover a single SG application can access different DCIs.|
||• SG user activity will be automatically tracked and usage resource automatically accounted.|

|**KF3**|**RESTful APIs**|
|---|--|
||•One of the most important feature of the FGF consists of the **[FutureGateway APIs](/fgfapis/)**. Any SG operation can be managed usign the FG APIs such as: application execution, check, status and results acquisition.|
||•The introduction of the REST APIs allow both back-end and front-end developers to target any kind of technology.|
||•Beside the tipical Science Gateway made of a web portal, mobile and desktop applications can be easily developed. Also workflow engines successfully exploited the FG APIs. In the same fashio IoT projects may get benefits from using the FGF.|
||•FGF provides APIs and libraries written for the most popular programming language to ease the use of APIs.|

[BREW]: https://brew.sh
[APACHE2]: https://www.apache.org/licenses/LICENSE-2.0
[GITHUB]: https://github.com
[G&CENG]: https://github.com/csgf/grid-and-cloud-engine/tree/FutureGateway
[JSAGA]: http://software.in2p3.fr/jsaga/latest-release/
[TOSCAORCH]: https://github.com/indigo-dc/orchestrator
[INDIGODC]: https://www.indigo-datacloud.eu