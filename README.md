FrontPage
=========
**The new dynamic face of dictyBase**


## Description
New design of the dictybase front-page to allow the integration of new features.

##### Web design
The new design will be developed according to the following basic objectives:

* Modernize the interface.
* Allow the integration of new technologies.
* Enable the expansion of new tools in the database.
* Facilitate the adaptation of current users.

The new front page will include:

* A header and footer shared by all the remaining pages.
* A picture box, which will include images of Dictyostelium.
* Direct link to the most popular resources of the dictybase.
* Editable content and other dynamic spaces (news, gadgets, events, etc)

##### Dynamic editable content

dictyBase contains a large portion of HTML pages that are handcrafted and maintained by manual edition on the server side. Both the edition of the content and the integration of third party widgets (such as twitter feed), are very difficult tasks under the current state.

[Raptor](https://www.raptor-editor.com/) will be used as the client HTML5 editor to make the content editable right from the browser (although other editors, as Mercury or bootstrap X-Editable, are not yet ruled out). The content will be pushed back and forth through a RESTful backend. The project will be split into the following sections:


- Define the content blocks and integrate the editor to make them editable.
- Use the [Rectangular framework](https://github.com/mgonto/restangular) (i.e., an [AngularJS](http://angularjs.org/) service to handle Rest API Restful Resources properly and easily) to save the edited content to a RESTful backend. 
- The RESTful backend (written in golang) and a HTTP resource as a deployable binary (*).
- Integrate image inclusion (explore AngularJS based option such as [Angular File Upload](https://github.com/danialfarid/angular-file-upload)).
- Editor available only to authorized users. For this, integrate the frontend to our RESTful authentication backend.

