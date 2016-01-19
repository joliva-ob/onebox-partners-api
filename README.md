FORMAT: 1A
HOST: http://onebox-partners-url/1.0/partners-api

# onebox-partners-api

## partners API
+ Manage a login into an external partner api
+ Get a list of events from an external partner filtered by an already logged client into that system
+ Handle to release an owned client seat from an external partner system
+ Handle to recover an owned client seat from an external partner system
+ Handle to change personal client access key from an external partner system

To do so, we have used a **API Blueprint** standard, **apiary** as an online editing and mocking tool, **aglio** to document it and **getsandbox** as a sandbox provider:
+ [API Blueprint](https://apiblueprint.org/)
+ [apiary.io](http://docs.oneboxpartnersapi.apiary.io/)
+ [getsandbox.com](http://onebox-partners-api.getsandbox.com/)
+ [aglio](https://github.com/danielgtaylor/aglio)
+ [github](https://github.com/joliva-ob/onebox-partners-api)
+ [onebox-developer](http://developer.oneboxtickets.com/partners-api/)

### Usage
1 edit the api blueprint document with apiary.io, or edit directly with Atom + blueprint plugin preview, language and lintr validation. This will provide a .md or .apib file.

2 generate the documentation from the .apib file with aglio:
```
aglio -i onebox-partners-api.apib -o welcome.html
```
from the command line.

3 update the online mock service by singin at https://getsandbox.com, going to onebox-partners-api and re-importing source from the .apib file. And finally, mock will be available for testing at: http://onebox-partners-api.getsandbox.com/<path_api>, ie: /dynamic-pricing-api/1.0/prices from any browser, curl -X, postman or soapui.

4 Apiary.io is already connected with github, so should be already up to date.
